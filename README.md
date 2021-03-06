# MyMusicList

MyMusicList is a minimalist Flask web-application that allows you to quickly deploy, host, and remotely manage your personal music playlist. MyMusicList utilizes youtube-dl to allow you to remotely download your favorite songs directly from YouTube and maintains all of your data in a lightweight SQLite database using PyDAL. 


## Features
* Music Player
* Add Song
* Remove Song
* Rename Song

## Get Started

1. Clone the repository 
```
git clone https://github.com/Snaacky/MyMusicList.git
```

2. Install the prerequisites
```
pip install -r requirements.txt
```

3. Update your Flask secret key to something unique in `mymusiclist.py`
```
app.config["SECRET_KEY"] = "PUT_YOUR_OWN_SECURE_KEY_HERE"
```

4. Update the path you plan to download to and store your music at in `mymusiclist.py` 
```
app.config["SONGS_PATH"] = "static/music/"
```

5. Execute the entrypoint.
```
python wsgi.py
```

## Requirements
* Python 3
* [Flask](https://github.com/pallets/flask)
* [PyDAL](https://github.com/web2py/pydal)
* [youtube-dl](https://github.com/ytdl-org/youtube-dl)

## Built With
* [audio.js](https://kolber.github.io/audiojs/)
* [Bootstrap 4](https://getbootstrap.com/)
