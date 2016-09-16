# Install Couchbase Server #

* Log-in into <a href="http://nitrous.io" target="_blank">Nitrous</a>/<a href="http://c9.io" target="_blank">Cloud9</a> environments
* Open IDE for the project
* Let's install Couchbase Serer using command line, <a href="http://developer.couchbase.com/documentation/server/current/getting-started/installing.html" target="_blank">vendor instructions</a>    
* Finding out libssl library we should install. Using terminal window/panel type: 
```
sudo apt-cache search libssl 
```  
* Result should look like:
```
libssl1.0.0 - Secure Sockets Layer toolkit - shared libraries
libssl-doc - Secure Sockets Layer toolkit - development documentation
libssl-dev - Secure Sockets Layer toolkit - development files
```
  
* Install libssl by typing in terminal window, it maybe install already - just to make sure:
```
sudo apt-get install libssl1.0.0
```
  
* Download Couchbase Server using terminal window by typing:
```
wget https://github.com/vkhazin/couchbase-courseware/raw/master/software/couchbase-server-enterprise_4.5.0-ubuntu14.04_amd64.deb
# or from backup location:  
# wget https://bitbucket.org/crsware/couchbase-courseware/raw/3bc2dd93831b5ac15decb927157deeaa37ee6350/software/couchbase-server-enterprise_4.5.0-ubuntu14.04_amd64.deb  
```

* Install Couchbase Server using terminal:
```
sudo dpkg -i ./couchbase-server-enterprise_4.5.0-ubuntu14.04_amd64.deb
```

* Check Admin ui is now accessible using terminal window:
```
curl localhost:8091
```

* Expected output:
```
<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html>
	<head><title>301 Moved Permanently</title></head>
	<body>
		<h1>Moved Permanently</h1>
		<p>The document has moved
			<a href="http://localhost:8091/ui/index.html>here</a>.
		</p>
	</body>
</html>
```

* From Nitrous top menu select 'Preview->(any option)'
* In the browser address bar add port info e.g.:
```
http://couchbase-courseware-213242.nitrousapp.com:8091/
```

* After a bit admin ui will show, select 'Setup' button
* Choose 'Start a new cluster' radio button
* Reduce 'Data RAM Quota:' and 'Index RAM Quota:' values to 256 - we are on small footprint sandbox here
* Replace hostname with the domain name <a style="color:red">(exclude protocol and port)</a> you see in the browser bar e.g.:
```
couchbase-courseware-213242.nitrousapp.com
```
  


