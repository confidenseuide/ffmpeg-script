# ffmpeg-script

`ffmpeg -i "/storage/emulated/0/DCIM/Camera/input.mp4" -vf "scale=-2:720,fps=fps=source_fps/2" -c:v libx265 -crf 28 -an "/storage/emulated/0/DCIM/Camera/output.mp4"`

En:
In my opinion, this is the best video compression script. (Besides compression, it removes sound.)

Ru:
Как по мне, лучший скрипт для сжатия видео. (Помимо сжатия он убирает звук.)

if you wanna with sound (если хотите со звуком):

`ffmpeg -i "/storage/emulated/0/DCIM/Camera/input.mp4" -vf "scale=-2:720,fps=fps=source_fps/2" -c:v libx265 -crf 30 -c:a libopus -b:a 64k "/storage/emulated/0/DCIM/Camera/output.mp4"`

Ru: Почему в версии со звуком больше сжатие видеоряда? Чтобы компенсировать добавление звука, а также потому что звук добавляет смысловую нагрузку к видеоряду, и его проще понять даже при низкой четкости.

En: Why in the version with sound is more compression of the video sequence? To compensate the addition of sound, and also because sound adds semantic load to the video sequence, and it is easier to understand even at low clarity.
