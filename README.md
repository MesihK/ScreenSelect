## About ScreenSELect
This tool allows you to select a rectangle on your screen which then can be used 
to record that portion of the screen via ffmpeg (x11grab) using the command

```
ffmpeg -f x11grab -framerate 25 $(./ssel) $(date+%Y-%m-%d_%H-%M_%S).mp4
```

You can compile the program using
```
gcc -Wall -lX11 ssel.c -o ssel
```

## Credits

The source code is from [this](https://bbs.archlinux.org/viewtopic.php?id=85378) forum post.
I just commented the code that grabs the keyboard.

