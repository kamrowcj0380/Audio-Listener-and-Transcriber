# Audio Listener and Transcriber
## Project Intention
The goal of this project is to pull audio streams (and possibly the audio component of video streams) from URLs, and listen to the audio as a live transcript is displayed on screen.

## Index

* [How To Run Locally](#run-local)
* [TODO List](#todo-list)


## <a id="run-local"></a> How To Run Locally

* Clone repo and open terminal in folder "audio_listener_and_transcriber/"
* Create virtual environment: $python -m venv virtual_env
* Activate virtual environment
  * In windows: $ .\virtual_env\Scripts\activate
  * In linux: $ source virtual_env/bin/activate
* Install modules to virtual environment from file
  * $ pip install -r requirements.txt
* Run this in the command line
```python 
$ python -c 'from django.core.management.utils import get_random_secret_key; print(get_random_secret_key())' > key.txt
```
* Copy the output from "key.txt" (and delete the file)
* Navigate to "audio_listener_and_transcriber\settings.py"
* Find the line below
```python
SECRET_KEY = os.getenv("KEY")
```
* Replace with the line below, replacing KEY with the key copied from "key.txt"
```python 
SECRET_KEY = "KEY"
```

* Run the Django server
```
$ python manage.py runserver
```
* Open a web browser, and navigate to server (http://127.0.0.1:8000/)


## <a id="todo-list"></a> TODO List 

* make TODO list
* The above is a joke, but true. Project designs will be created and added

