### View tag on client opened

DWM patch that brings this common wm functionality to switch focus to the tag where a new client window was spawned. 

---

Dwm already provides the way to specify on which tag the client window of some type should appear.  
However the client's rules definition isn't extensible at all as it comes as a predefined struct in C source code.  
So this patch brings one more dwm rules customization option called ```viewtag```. Provided a non 0 value it will switch  
focus to the specified tag for all client instances of provided client type.

---
To apply the patch:
```
wget https://raw.githubusercontent.com/slamko/dwm-viewtag-on-client-open/master/dwm-viewtag_on_client_open-6.3.diff &&
patch < dwm-viewtag_on_client_open-6.3.diff
```
