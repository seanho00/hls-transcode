# hls-transcode
Transcode MP4 video to adaptive bitrate HLS.

Original motivation was for family videos on nextCloud, VOD from mobile devices.

## Usage
```
hls-transcode <input MP4 videos>
```

## Output
Master HLS playlist for each video takes same name as video, with `.m3u8` extension.

Bitrate-specific playlists and transcoded videos are in subdirs under `.hls` in the current directory,
named after each video file.

## Options
To edit the resolution and bitrates, edit the `bitrate` dictionary near the top of the script.

## References
+ https://ffmpeg.org/ffmpeg-formats.html#hls-2
+ https://github.com/bentasker/HLS-Stream-Creator
