### home
- jobs
	- 3x apps
		- Chelsea's ARL writing role
		- other ARL role
	- Docker --> Kubernetes exercise for profilometer
		- come up with ideas to chat with Ben about for coding work experience
- sweeping, mowing
- CRV engine
- groceries
- batch migrating ownership of projects between github accounts
- Ask Seana what time her recital is (Thurs 28th at The Shop)

### work
- purchases
	- Kingston v90 storage ($70 - [amazon](https://www.amazon.com/Kingston-Canvas-64GB-UHS-II-SDR2/dp/B09XC5GG83/ref=sr_1_7?sr=8-7))
	- LEDs ($120 - 60 W LED (flickerless) - [ebay](https://www.ebay.com/itm/356119918728?chn=ps&google_free_listing_action=view_item))
	- 52 mm RX100 filter adapter (???)
	- **Raynox DCR-250** ($75 - [B&H](https://www.bhphotovideo.com/c/product/275182-REG/Raynox_DCR_250_DCR_250_2_5x_Super_Macro.html?ap=y&smp=Y)) 
	- cheap welding gas flow gear
	- ebay flow chamber gear
- next slow mo camera
	- change slow mo time (supposedly higher res at 2 s vs 4 s)

# HFR CLI processing pipeline (ffmpeg)
### process original file for sharing
```shell
ffmpeg -ss 00:00:00 -t 30 -i input.mp4 -vf "scale=iw/2:ih/2,setpts=2.4975*PTS" -r 24 -c:v libx264 -pix_fmt yuv420p -an output.mp4
```
here, crop the first 30s,  0.5x the resolution, and convert the codec to h.264
- ffmpeg '-ss'+'-t',  '-vf', and '-c:v' commands respectively
- size ~400 MB -> ~7 MB
### add timer overlay with 
```shell
ffmpeg -i input.mp4 -vf "drawtext=fontfile='C\:/Windows/Fonts/consola.ttf':text='%{eif\:floor((t/40)/3600)\:d\:2}\:%{eif\:mod(floor((t/40)/60)\,60)\:d\:2}\:%{eif\:mod(floor(t/40)\,60)\:d\:2}':x=w-tw-20:y=20:fontsize=24:fontcolor=white:box=1:boxcolor=black@0.55:boxborderw=8" -c:v libx264 -crf 18 -preset medium -c:a output.mp4
```
here, 960 fps -> 24 fps = 1/40
- uses ffmpeg '-vf drawtext' 
### troubleshooting - reveal codec
```bash
ffprobe -v error -select_streams v:0 -show_entries stream=codec_name -of default=noprint_wrappers=1:nokey=1 input.mp4
```
- uses 'ffprobe -show_entries'
- should output "h264" after above commands
### add audio
```shell
ffmpeg -i input_video.mp4 -ss 10 -i input_audio.wav -map 0:v:0 -map 1:a:0 -c:v copy -c:a aac -b:a 192k -shortest output_with_audio.mp4
```
asdf