# XsSpotter
XsSpotter is a powerful tool designed for automatic XSS detection in web applications built on the popular tool XssPy. This tool has been used to find vulnerabilities in multiple high traffic sites.

## Description
XsSpotter can be used to detect a multitude of common XSS vulnerabilities in web applications. It has the capabilities of detecting:
* XSS through input fields
* XSS through URL parameters
* Unescaped characters

After finding a possible vulnerable input, XsSpotter will rank the possibility of exploitability on a scale of high, medium, to low. These inputs will then be printed after testing with the payload used.

XsSpotter also presents a dynamic dashboard with live updates of testing. Any time a vulnerable area is found it will be outputted to the console for immediate testing so there is no need to wait for large sites to finish.
 ![alt text](http://XsSpotterDash.png)

## Usage
To print out the help menu, use the -h flag
```
python XsSpotter.py -h
```
Using XsSpotter is as easy as just adding a site to test on
```
python XsSpotter.py -u <site to test (http(s) removed)>
```
Add the -e flag to traverse the site even deeper
```
python XsSpotter.py -u <site> -e
```
The -v flag will add testing for XSS in url parameters as well
```
python XsSpotter.py -u <site> -v
```
