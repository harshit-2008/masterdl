run command 
cd Your Folder/N_m3u8DL-RE.exe

run commands :-
Description:
  N_m3u8DL-RE (Beta version) 20230412

Usage:
  N_m3u8DL-RE <input> [options]

Arguments:
  <input>  Input Url or File

Options:
  --tmp-dir <tmp-dir>                      Set temporary file directory
  --save-dir <save-dir>                    Set output directory
  --save-name <save-name>                  Set output filename
  --base-url <base-url>                    Set BaseURL
  --thread-count <number>                  Set download thread count [default: 4]
  --download-retry-count <number>          The number of retries when download segment error [default: 3]
  --auto-select                            Automatically selects the best tracks of all types [default: False]
  --skip-merge                             Skip segments merge [default: False]
  --skip-download                          Skip download [default: False]
  --check-segments-count                   Check if the actual number of segments downloaded matches the expected
                                           number [default: True]
  --binary-merge                           Binary merge [default: False]
  --del-after-done                         Delete temporary files when done [default: True]
  --no-date-info                           Date information is not written during muxing [default: False]
  --write-meta-json                        Write meta json after parsed [default: False]
  --append-url-params                      Add Params of input Url to segments, useful for some websites, such as
                                           kakao.com [default: False]
  -mt, --concurrent-download               Concurrently download the selected audio, video and subtitles [default:
                                           False]
  -H, --header <header>                    Pass custom header(s) to server, Example:
                                           -H "Cookie: mycookie" -H "User-Agent: iOS"
  --sub-only                               Select only subtitle tracks [default: False]
  --sub-format <SRT|VTT>                   Subtitle output format [default: SRT]
  --auto-subtitle-fix                      Automatically fix subtitles [default: True]
  --ffmpeg-binary-path <PATH>              Full path to the ffmpeg binary, like C:\Tools\ffmpeg.exe
  --log-level <DEBUG|ERROR|INFO|OFF|WARN>  Set log level [default: INFO]
  --ui-language <en-US|zh-CN|zh-TW>        Set UI language
  --urlprocessor-args <urlprocessor-args>  Give these arguments to the URL Processors.
  --key <key>                              Pass decryption key(s) to mp4decrypt/shaka-packager. format:
                                           --key KID1:KEY1 --key KID2:KEY2
  --key-text-file <key-text-file>          Set the kid-key file, the program will search the KEY with KID from the
                                           file.(Very large file are not recommended)
  --decryption-binary-path <PATH>          Full path to the tool used for MP4 decryption, like C:\Tools\mp4decrypt.exe
  --use-shaka-packager                     Use shaka-packager instead of mp4decrypt to decrypt [default: False]
  --mp4-real-time-decryption               Decrypt MP4 segments in real time [default: False]
  -M, --mux-after-done <OPTIONS>           When all works is done, try to mux the downloaded streams. Use "--morehelp
                                           mux-after-done" for more details
  --custom-hls-method <METHOD>             Set HLS encryption method
                                           (AES_128|AES_128_ECB|CENC|CHACHA20|NONE|SAMPLE_AES|SAMPLE_AES_CTR|UNKNOWN)
  --custom-hls-key <FILE|HEX|BASE64>       Set the HLS decryption key. Can be file, HEX or Base64
  --custom-hls-iv <FILE|HEX|BASE64>        Set the HLS decryption iv. Can be file, HEX or Base64
  --use-system-proxy                       Use system default proxy [default: True]
  --custom-proxy <URL>                     Set web request proxy, like http://127.0.0.1:8888
  --task-start-at <yyyyMMddHHmmss>         Task execution will not start before this time
  --live-perform-as-vod                    Download live streams as vod [default: False]
  --live-real-time-merge                   Real-time merge into file when recording live [default: False]
  --live-keep-segments                     Keep segments when recording a live (liveRealTimeMerge enabled) [default:
                                           True]
  --live-pipe-mux                          Real-time muxing to TS file through pipeline + ffmpeg (liveRealTimeMerge
                                           enabled) [default: False]
  --live-fix-vtt-by-audio                  Correct VTT sub by reading the start time of the audio file [default: False]
  --live-record-limit <HH:mm:ss>           Recording time limit when recording live
  --live-wait-time <SEC>                   Manually set the live playlist refresh interval
  --mux-import <OPTIONS>                   When MuxAfterDone enabled, allow to import local media files. Use
                                           "--morehelp mux-import" for more details
  -sv, --select-video <OPTIONS>            Select video streams by regular expressions. Use "--morehelp select-video"
                                           for more details
  -sa, --select-audio <OPTIONS>            Select audio streams by regular expressions. Use "--morehelp select-audio"
                                           for more details
  -ss, --select-subtitle <OPTIONS>         Select subtitle streams by regular expressions. Use "--morehelp
                                           select-subtitle" for more details
  -dv, --drop-video <OPTIONS>              Drop video streams by regular expressions.
  -da, --drop-audio <OPTIONS>              Drop audio streams by regular expressions.
  -ds, --drop-subtitle <OPTIONS>           Drop subtitle streams by regular expressions.
  --morehelp <OPTION>                      Set more help info about one option
  --version                                Show version information
  -?, -h, --help                           Show help and usage information
