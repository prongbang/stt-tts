# Speak to Text and Text to Speak on Web Application

## Import library
```html
<script src="http://code.responsivevoice.org/responsivevoice.js"></script>
```

## New Instance `webkitSpeechRecognition` and Configuration
```js
responsiveVoice.setDefaultVoice("Thai Female");
var recognition = new webkitSpeechRecognition();
recognition.continuous = false;
recognition.interimResults = true;
recognition.lang = 'th-TH';
```

## Speak to Text listening
```js
recognition.onstart = function () { };

recognition.onerror = function (event) { };

recognition.onend = function () { }

recognition.onresult = function (event) { };
```

## Start
```js
recognition.start();
```

## Start
```js
recognition.stop();
```

## Text to Speak
```js
responsiveVoice.speak("message", "Thai Female", {pitch: 1.1});
```