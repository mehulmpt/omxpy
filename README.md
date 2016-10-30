# omxpy

omxpy makes it easier to use omxplayer with remote python script control. It requires **pexpect** module installed.

# Usage

*script.py*
```python
from omxpy import omxpy

#... after some code
omx = OMXPlayer("./Movies/movie.mp4")
omx.toggle_pause()
omx.jump30s()
# ...
```

**Warning: ** This module runs on the same thread as that of the calling python script. Make sure to place it in another thread if you're looking for non-blocking python script.
