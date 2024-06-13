# YouTube Video Downloader

A simple GUI-based YouTube video downloader for Windows built using Python and Tkinter. It allows users to download YouTube videos in MP4 or MP3 format and select the download location. It also supports downloading multiple videos from a text file.

## Features
- Download YouTube videos in MP4 or MP3 format
- Select the download location
- Fetch YouTube video thumbnail automatically
- Download multiple videos from a text file containing YouTube URLs

## Built App
The pre-built App is located in the output folder and can be executed directly.

## Requirements for development
- Python 3.x
- pytube package
- tkinter (included with Python)
- pillow package
- requests package
- certifi package

## Usage
Install the required packages mentioned above. You can install them using pip:
```
pip install pytube pillow requests certifi
```
Run `youtube_downloader.py`:
```
python youtube_downloader.py
```
Enter the YouTube video URL in the text box.

Select the desired format: MP4 or MP3.

Click "Select Download Location" to choose the download folder.

Click "Download" to start downloading the video.

### Downloading Multiple Videos
Prepare a text file with one YouTube URL per line.

Click "Download from File" in the application.

Select the text file containing YouTube URLs.

The application will download all videos sequentially.

## How do I run the app in docker?

```
docker run -it --rm --name youtube-downloader -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix youtube-downloader
```

## License
This project is released under the MIT License.
