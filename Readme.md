*This repository is a mirror of the [component](http://component.io) module [bmcmahen/auto-save](http://github.com/bmcmahen/auto-save). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/bmcmahen-auto-save`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# auto-save

  A simple timer wrapper that is useful for implementing a delayed autosave in text-based applications, like Google Docs. 

## Installation

  Install with [component(1)](http://component.io):

    $ component install bmcmahen/auto-save

## API

```javascript
// 500 represents the timeout duration in ms.
var autosave = require('auto-save')(500);
var txt = document.getElementByTagName('textarea')[0];
txt.oninput = function(){
  interval(function(){
    console.log('do some saving.');
  });
};
```

## License

  MIT
