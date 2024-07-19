`astiav-rockchip` is fork from a Golang library `go-astiav` providing C bindings for [ffmpeg-rockchip](https://github.com/nyanmisaka/ffmpeg-rockchip)

It's only compatible with `ffmpeg-rochckip`.

Its main goals are to:

- [x] provide a better GO idiomatic API
    - standard error pattern
    - typed constants and flags
    - struct-based functions
    - ...
- [x] provide the GO version of [ffmpeg examples](https://github.com/FFmpeg/FFmpeg/tree/n6.1.1/doc/examples)
- [x] be fully tested

# Examples

Examples are located in the [examples](examples) directory and mirror as much as possible the [ffmpeg examples](https://github.com/FFmpeg/FFmpeg/tree/n6.1.1/doc/examples).

|name|astiav|ffmpeg|
|---|---|---|
|Demuxing/Decoding|[see](examples/demuxing_decoding/main.go)|[see](https://github.com/FFmpeg/FFmpeg/blob/n6.1.1/doc/examples/demuxing_decoding.c)
|Filtering|[see](examples/filtering/main.go)|[see](https://github.com/FFmpeg/FFmpeg/blob/n6.1.1/doc/examples/filtering_video.c)
|Hardware Decoding|[see](examples/hardware_decoding/main.go)|[see](https://github.com/FFmpeg/FFmpeg/blob/n6.1.1/doc/examples/hw_decode.c)
|Remuxing|[see](examples/remuxing/main.go)|[see](https://github.com/FFmpeg/FFmpeg/blob/n6.1.1/doc/examples/remuxing.c)
|Scaling|[see](examples/scaling/main.go)|[see](https://github.com/FFmpeg/FFmpeg/blob/n6.1.1/doc/examples/scaling_video.c)
|Transcoding|[see](examples/transcoding/main.go)|[see](https://github.com/FFmpeg/FFmpeg/blob/n6.1.1/doc/examples/transcoding.c)

*Tip: you can use the video sample located in the `testdata` directory for your tests*

# Install ffmpeg from source

https://github.com/nyanmisaka/ffmpeg-rockchip/wiki/Compilation

# Why astiav-rockchip?

After several months of continuous effort and failure, I almost gave up on further development of [go-rkcodec](github.com/Tryanks/go-rkcodec). Now, I want to adapt the code to ffmpeg-rockchip.