# Using YouTube-DL from the Command Line

# Installation:

## To install `youtube-dl` , we use the command:

### (Ensure that Python is installed globally)

```powershell
pip install --no-cache-dir youtube-dl
```

# Usage:

## To use youtube-dl, open a shell (as Administrator) and navigate to the directory where you want to store the music using the `cd` command.

### Open either [music.youtube.com](http://music.youtube.com) or [https://www.youtube.com/](https://www.youtube.com/) and search for your video/song. Copy the link of the video/song using the **`Share` button.**

## Open your shell and type this command:

```powershell
youtube-dl -o "%(title)s.%(ext)s" -x --audio-format flac --audio-quality 0 {LINK}
```

Replace {LINK} with the link that you copied.

## **Ensure that there is no ampersand operator [&] in the link. For example,**

If the Link copied is this:

[`https://music.youtube.com/watch?v=-mLpe7KUg9U&feature=share`](https://music.youtube.com/watch?v=-mLpe7KUg9U&feature=share)

Remove everything that comes after the ampersand. So, the link should look like this at the end:

[`https://music.youtube.com/watch?v=-mLpe7KUg9U`](https://music.youtube.com/watch?v=-mLpe7KUg9U&feature=share)