php curl 모바일 url
```
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, $url);
curl_setopt($ch, CURLOPT_HEADER, true);
curl_setopt($ch, CURLOPT_FOLLOWLOCATION, false);
curl_setopt($ch, CURLOPT_RETURNTRANSFER, TRUE);
curl_setopt($ch, CURLOPT_TIMEOUT_MS, 1000);
curl_setopt($ch,CURLOPT_USERAGENT,'User-Agent: Mozilla/5.0 (iPhone; CPU iPhone OS 10_0_1 like Mac OS X) AppleWebKit/602.1.50 (KHTML, like Gecko) Version/10.0 Mobile/14A403 Safari/602.1');
$result = curl_exec($ch);
$httpStatus = curl_getinfo($ch, CURLINFO_HTTP_CODE);
curl_close($ch);

// if it's not a redirection (3XX), move along
if ($httpStatus < 300 || $httpStatus >= 400)
$result =  "location:".$url;

// look for a location: header to find the target URL
if(preg_match('/location: (.*)/i', $result, $r)) {
$location = trim($r[1]);

// if the location is a relative URL, attempt to make it absolute
if (preg_match('/^\/(.*)/', $location)) {
    $urlParts = parse_url($url);
    if ($urlParts['scheme'])
	$baseURL = $urlParts['scheme'].'://';
    else
	$baseURL = 'http://';

    if ($urlParts['host'])
	$baseURL .= $urlParts['host'];
    else
	$baseURL .= $url;

    if ($urlParts['port'])
	$baseURL .= ':'.$urlParts['port'];

    return $baseURL.$location;
}

return $location;
}
return $url;
```
php memory check
```
$file = fopen($_FILES[$filename]['tmp_name'], 'rb');
if ($file == false) {
return false;
}

$filesize = filesize($_FILES[$filename]['tmp_name']);
$buffersize = 2048;
if (memory_get_usage() && ($memory_limit = ini_get('memory_limit')) > 0) {
$memory_limit = str_split($memory_limit, strspn($memory_limit, '1234567890'));
if ( ! empty($memory_limit[1])) {
    switch ($memory_limit[1][0])
    {
	case 'g':
	case 'G':
	    $memory_limit[0] *= 1024 * 1024 * 1024;
	    break;
	case 'm':
	case 'M':
	    $memory_limit[0] *= 1024 * 1024;
	    break;
	default:
	    break;
    }
}

$memory_limit = (int) ceil($filesize + $buffersize + $memory_limit[0]);
ini_set('memory_limit', $memory_limit); // When an integer is used, the value is measured in bytes. - PHP.net
}

$nospacetext = '';
while(!feof($file)) {
$filetext = fread($file, $buffersize);
$nospacetext .= preg_replace('/\s+/', '', $filetext);
}
fclose($file);
return ! preg_match('/<(body|head|html|img|plaintext|pre|script|table|title|object|iframe|style)>|<\?php/i', $nospacetext);
```
