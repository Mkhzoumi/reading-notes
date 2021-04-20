# *local storage of web application*
## *in the past web application were use cookies for presistent local storage of small amount of data, but cookies have three dealbreaking:*
1. ## *Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.*
2. ## *Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL).*
3. ## *Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.*

## *HTML5 storage:  it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you.*

```
             HTML5 STORAGE SUPPORT

 IE   FIREFOX   SAFARI	CHROME	OPERA	IPHONE	ANDROID
8.0+	3.5+	4.0+	4.0+	10.5+	2.0+	2.0+
```

## *you can access html5 storage through the localstorage object on the global window object using javascript, but first you have to check wether the browser support it.*

```
function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}

OR

if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
}
```

## *Web SQL Database (formerly known as “WebDB”) provides a thin wrapper around a SQL database, allowing you to do things like this from JavaScript:*

```
openDatabase('documents', '1.0', 'Local document storage', 5*1024*1024, function (db) {
  db.changeVersion('', '1.0', function (t) {
    t.executeSql('CREATE TABLE docids (id, name)');
  }, error);
});
```

## *in web sql "WebDB" most of the action resides in the string you pass to the executeSql method. This string can be any supported SQL statement including SELECT, UPDATE, INSERT, and DELETE statements. It’s just like backend database programming, except you’re doing it from JavaScript*

## *there are four browsers support Web SQL:*

```
          WEB SQL DATABASE SUPPORT

	SAFARI	CHROME	OPERA	IPHONE	ANDROID
     4.0+	 4.0+	10.5+	3.0+	2.0+
```

# [back](../README.md)