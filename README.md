# mergeVideoFFmpegCommand
merge video working FFmpeg command :

# '-y -i $firstVideoPath -i $videoPath -r 24000/1001 -filter_complex "[0:v]scale=1080:1920, fps=30[v0];[1:v]scale=1080:1920, fps=30[v1];[v0][0:a][v1][1:a]concat=n=2:v =1:a=1[outv][outa]" -map "[outv]" -map "[outa]" -vsync 2 $outputPath'  


