# Original 7DRL Release
These binaries were released before the deadline for the 7DRL challenge. As such, they can be considered the official releases if you're strict on the definitions of the rules.

However, due to an oversight during development, these binaries likely require at least a 720p monitor to play (only tested on 1080p and 15" Retina). This is much for many monitors, and so "resolution fixed" versions were released on the day after (2017-03-12) which may be more appropriate for a wider range of monitors. See the root of this repository for details.

## It won't Work!
See the README at the root of this repository for details on what you might need to do.

## What's "NativeArch"?
The Ubuntu binaries were intitially compiled with `-march=native` which caused instructions specific to the i5-4590 CPU to be generated. This isn't portable to platforms which don't have the same instruction set. As such, the NativeArch version was the initial Ubuntu release, but the `ubuntu16.10` version should be the version you use. The NativeArch version is kept for reference (and, if you happen to have a compatible processor, it'll be a little faster too)
