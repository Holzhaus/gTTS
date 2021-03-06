gTTS
====

**gTTS** (Google Text to Speech): a Python interface to Google's Text to Speech API. Create an mp3 file with the `gTTS` module or `gtts-cli` command line utility. It allows for unlimited lengths of spoken text by tokenizing long sentences where the speech would naturally pause.

[![Build Status](https://travis-ci.org/pndurette/gTTS.svg?branch=master)](https://travis-ci.org/pndurette/gTTS)

Install
-------

    pip install gTTS

Module
------

Instanciate:

    >> from gtts import gTTS
    >> tts = gTTS(text='Hello', lang='en')
    >> tts.save("hello.mp3")

**Parameters**:

  *  `text` is the text to speak to file;
  *  `lang` is the language to speak in. A ISO 639-1 language code supported by the Google Text to Speech API.

Command line utility
--------------------
Invoke `gtts-cli`:

    gtts-cli.py --help
    usage: gtts-cli.py [-h] (-t TEXT | -f FILE) [-l LANG] [--debug] destination

(Ex.) Read the string 'Hello' in English to hello.mp3

    $ gtts-cli.py -t "Hello" -l 'en' hello.mp3

(Ex.) Read the contents of file 'hello.txt' in Czech to hello.mp3:

    $ gtts-cli.py -f hello.txt -l 'cs' hello.mp3

Supported Languages
-------------------

  * 'af' : 'Afrikaans'
  * 'sq' : 'Albanian'
  * 'ar' : 'Arabic'
  * 'hy' : 'Armenian'
  * 'ca' : 'Catalan'
  * 'zh' : 'Chinese',
  * 'zh-cn' : 'Chinese (Mandarin/China)'
  * 'zh-tw' : 'Chinese (Mandarin/Taiwan)'
  * 'zh-yue' : 'Chinese (Cantonese)'
  * 'hr' : 'Croatian'
  * 'cs' : 'Czech'
  * 'da' : 'Danish'
  * 'nl' : 'Dutch'
  * 'en' : 'English'
  * 'en-au' : 'English (Australia)'
  * 'en-uk' : 'English (United Kingdom)'
  * 'en-us' : 'English (United States)'
  * 'eo' : 'Esperanto'
  * 'fi' : 'Finnish'
  * 'fr' : 'French'
  * 'de' : 'German'
  * 'el' : 'Greek'
  * 'ht' : 'Haitian Creole'
  * 'hi' : 'Hindi'
  * 'hu' : 'Hungarian'
  * 'is' : 'Icelandic'
  * 'id' : 'Indonesian'
  * 'it' : 'Italian'
  * 'ja' : 'Japanese'
  * 'ko' : 'Korean'
  * 'la' : 'Latin'
  * 'lv' : 'Latvian'
  * 'mk' : 'Macedonian'
  * 'no' : 'Norwegian'
  * 'pl' : 'Polish'
  * 'pt' : 'Portuguese'
  * 'pt-br' : 'Portuguese (Brazil)'
  * 'ro' : 'Romanian'
  * 'ru' : 'Russian'
  * 'sr' : 'Serbian'
  * 'sk' : 'Slovak'
  * 'es' : 'Spanish'
  * 'es-es' : 'Spanish (Spain)'
  * 'es-us' : 'Spanish (United States)'
  * 'sw' : 'Swahili'
  * 'sv' : 'Swedish'
  * 'ta' : 'Tamil'
  * 'th' : 'Thai'
  * 'tr' : 'Turkish'
  * 'vi' : 'Vietnamese'
  * 'cy' : 'Welsh'

