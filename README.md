# Overview
Golang lightweight log component, support level control, file log...

Getting Started
---------------

```go
package main

import (
	log "github.com/Kuloud/Klog"
)

func main() {
	log.V("vTag", "hello", "kuloud")
	log.Vf("vfTag", "%s, just like %s said.", "hello", "kuloud")
	log.D("dTag", "hello", "kuloud")
	log.Df("dfTag", "%s, just like %s said. %d", "hello", "kuloud", 1)
	log.I("iTag", "hello", "kuloud")
	log.If("ifTag", "%s, just like %s said. %t", "hello", "kuloud", true)
	log.W("wTag", "hello", "kuloud")
	log.Wf("wfTag", "%s, just like %s said. %s", "hello", "kuloud", "Debug")
	log.E("eTag", "hello", "kuloud")
	log.Ef("efTag", "%s, just like you said.")
}

```


Installation and Upgrade
------------------------

```
$ go get -u github.com/Kuloud/Klog
```

History
-------

v1.0.0, 7 Nov 2015
------------------
* Initial release
** Level contorl
** File log


License
-------

Apache License Version 2.0. See [LICENSE](https://github.com/Kuloud/Klog/blob/master/LICENSE) file for details.


ToDo
----
* Load configuration by profile, such as xml/properties... Fix log file recreate each time.

