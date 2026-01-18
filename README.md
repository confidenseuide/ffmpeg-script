# ffmpeg-script

`ffmpeg -i "/storage/emulated/0/DCIM/Camera/input.mp4" -vf "scale=-2:720,fps=fps=source_fps/3" -c:v libx265 -crf 28 -an "/storage/emulated/0/DCIM/Camera/output.mp4"`

En:
In my opinion, this is the best video compression script. (Besides compression, it removes sound.)

Ru:
Как по мне, лучший скрипт для сжатия видео. (Помимо сжатия он убирает звук.)
