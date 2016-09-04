# ffmpeg-android-build

Build script for cross compile ffmpeg for Android. It generates libs for all platforms (except 64 bit).

Works with ffmpeg 3.1 and Android NDK r11b.

Now ffmpeg support native decoding using MediaCodec!

Example usage here: https://github.com/HausnerR/ffmpeg-android-example.

## Requirements

Installed Android NDK and propably that's all.

## Howto

1. Clone this repo
2. Execute *git submodule init && git submodule update*
3. Set **ANDROID_NDK_DIR** and **FEATURES** in build.sh
4. Run *./build.sh*
5. Static libraries should be generated and ready to use in *android-builds* directory

## Features

Default defined **FEATURES** in build.sh are only for local mp4 video playing!
If you want more features like another formats, protocols, encoding, whatever - modify this variable.

## Inspiration

- http://enoent.fr/blog/2014/06/20/compile-ffmpeg-for-android/
- https://github.com/appunite/AndroidFFmpeg
