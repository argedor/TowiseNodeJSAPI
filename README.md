
# TOWISE NODE API
Towise assists you to detect human faces and bodies with using the latest and reliable technology.

## Getting Started
### Prerequisites 
```
 node v8+
 npm v3+

```
### Installing
To install the package

```
npm install towise 
```
To import your project
```
const Towise = require('towise');
```
### Using Towise
You must enter appKey and appId

For Example:
```
const Towise = require('towise');

const towise = new Towise({ 
    appID: 'type your appId', 
    appKey: 'type your appKey' 
    });

const image_url = "https://cdn.onebauer.media/one/media/5c6e/80bc/d007/9656/5f0a/6c12/dua-lipa-brits.jpg";

//for face detection
towise.faceDetect(image_url)
        .then( res => console.log(res))
        .catch( err => console.error(err));

//for body detection
towise.bodyDetect(image_url)
        .then( res => console.log(res))
        .catch( err => console.error(err));

//for emotion detection
towise.emotionDetect(image_url)
        .then( res => console.log(res))
        .catch( err => console.error(err));
```

## Versioning
For the versions available, see the https://github.com/argedor/TowiseNodeJSAPI/tags

## Authors
* **Harun Keleşoğlu** - *Developer* - [Github](https://github.com/harunkelesoglu)
See also the list of [contributers](https://github.com/argedor/TowiseNodeJSAPI/graphs/contributors)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details