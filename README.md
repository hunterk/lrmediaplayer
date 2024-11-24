#LRMediaPlayer

This is a standalone repo that tracks the RetroArch repo to build the ffmpeg-libretro core. This core is built into RetroArch, but there are plenty of reasons to want a separate core, mostly related to creating audio/video playlists via the 'manual scan' function and then associating this core with it, which is not possible with the built-in core.

##How to Build

Just go into the libretro-ffmpeg directory and invoke 'make,' like this:

    cd libretro-ffmpeg && make
    
The only dependencies are ffmpeg and libass development libraries (libass-dev).

Since it uses shared ffmpeg libs rather than statically linking, cores built on one person's system may not work on someone else's system, just fair warning.
