## About ##

matlabcontrol is a Java API that allows for calling MATLAB from Java. You can `eval`, `feval`, as well as get and set variables. Interaction can be performed from either inside MATLAB or outside MATLAB.

Version 4 adds many feature requests including reconnecting to a previously controlled MATLAB session, running MATLAB hidden, and better handling of returned data. To see exactly what has changed, consult the [version history](VersionHistory.md) page.

## Getting Started ##

The basic usage pattern with matlabcontrol is to create a factory, and then to create a proxy. The proxy is used to communicate with MATLAB.
```
MatlabProxyFactory factory = new MatlabProxyFactory();
MatlabProxy proxy = factory.getProxy();
...
//Use the proxy as desired
...
proxy.disconnect();
```
To find out how to use the proxy, start reading the walkthrough.

**[Walkthrough](http://code.google.com/p/matlabcontrol/wiki/Walkthrough)** - Explains how to use matlabcontrol.

**[javadocs](http://matlabcontrol.googlecode.com/svn/javadocs/doc/index.html)** - Full javadoc documentation of matlabcontrol.

**[FAQ](http://code.google.com/p/matlabcontrol/wiki/FAQ)** - Frequently (and some infrequently) asked questions about matlabcontrol.

## Bugs ##
If you encounter a bug, please [file it](https://code.google.com/p/matlabcontrol/issues/entry) with as much information as you have.

## Compatibility ##
This API relies upon the [Java MATLAB Interface](http://code.google.com/p/matlabcontrol/wiki/JMI) distributed with all recent copies of MATLAB. This interface is entirely undocumented and there is no guarantee matlabcontrol will work with all versions of MATLAB and operating systems. Efforts are made to ensure compatibility with MATLAB `R2007b` and greater, see [here](http://code.google.com/p/matlabcontrol/wiki/Compatibility) for specifics.

## Announcements ##

_March 1, 2013_

Version 4.1.0 has been released! It includes minor additions and bug fixes. See the [version history](VersionHistory.md) page for more information.

Older announcements can be found [here](Announcements.md).


---

_There are a variety of approaches to controlling MATLAB from Java, each with multiple solutions. To see which approach makes the most sense for your needs, please read [this page](http://code.google.com/p/matlabcontrol/wiki/ApproachesToControl) which provides overviews and links._

---


_The icon for matlabcontrol is part of the Um collection created by_<a href='http://mattahan.deviantart.com/'>mattahan (Paul Davey)</a>. It is licensed under the <a href='http://creativecommons.org/licenses/by-nc-sa/3.0/'>CC Attribution-Noncommercial-Share Alike 3.0 License</a>.