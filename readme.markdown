PHP simple cached cURL
======================
[Dirk Ginader](http://ginader.com/)

very simple wrapper for cURL that creates a local file cache

usage: created a folder named "cache" in the same folder as this file and chmod it 777
call this function with 2+1 parameters:

    $curlReturn = simpleCachedCurl($url,$expires,$debug);

    $url (string) the URL of the data that you would like to load
    $expires (integer) the amound of seconds the cache should stay valid
    $debug (boolean, optional) write debug information for troubleshooting

returns either the raw cURL data or false if request fails and no cache is available

Requirements
------------
* PHP cURL (php5-curl)
