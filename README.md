# tablette_tactile
Source code for tablette

Introduction

Tablette is a micro Python module to transform tabular data to nested lists of dicts.

Why

The purpose of the module is to make it easy to create JSON data starting from a database cursor. Yes. A database cursor, do you remember that? :)

How it works

As an example, consider this dataset:

columns = ['id', 'username', 'url_id', 'url', 'tag_id', 'tag']
data = [
        [ 1, 'albi', 1, 'http://python.org/', 1, 'programming language' ],
        [ 1, 'albi', 1, 'http://python.org/', 2, 'open source' ],
        [ 1, 'albi', 2, 'http://php.net/', 2, 'open source' ],
        [ 1, 'albi', 2, 'http://php.net/', 3, 'web' ],
        [ 2, 'karl', 3, 'http://reddit.com/', 4, 'lol' ],
        [ 2, 'karl', 3, 'http://reddit.com/', 5, 'wtf' ]
    ]
    
    // Include and instantiate the class.
require_once 'Mobile_Detect.php';
$detect = new Mobile_Detect;
 
// Any mobile device (phones or tablets).
if ( $detect->isMobile() ) {
 
}
 
// Any tablet device.
if( $detect->isTablet() ){
 
}
 
// Exclude tablets.
if( $detect->isMobile() && !$detect->isTablet() ){
 
}
 
// Check for a specific platform with the help of the magic methods:
if( $detect->isiOS() ){
 
}
 
if( $detect->isAndroidOS() ){
 
}
 
// Alternative method is() for checking specific properties.
// WARNING: this method is in BETA, some keyword properties will change in the future.
$detect->is('Chrome')
$detect->is('iOS')
$detect->is('UC Browser')
// [...]
 
// Batch mode using setUserAgent():
$userAgents = array(
'Mozilla/5.0 (Linux; Android 4.0.4; Desire HD Build/IMM76D) AppleWebKit/535.19 (KHTML, like Gecko) Chrome/18.0.1025.166 Mobile Safari/535.19',
'BlackBerry7100i/4.1.0 Profile/MIDP-2.0 Configuration/CLDC-1.1 VendorID/103',
// [...]
);
foreach($userAgents as $userAgent){
 
  $detect->setUserAgent($userAgent);
  $isMobile = $detect->isMobile();
  $isTablet = $detect->isTablet();
  // Use the force however you want.
 
}
 
// Get the version() of components.
// WARNING: this method is in BETA, some keyword properties will change in the future.
$detect->version('iPad'); // 4.3 (float)
$detect->version('iPhone') // 3.1 (float)
$detect->version('Android'); // 2.1 (float)
$detect->version('Opera Mini'); // 5.0 (float)

With this code, you will be able to know how to use a [tablette tactile](https://www.besttech.fr) easily. And you will be able to detect if your visitor uses a tablette on your website.
