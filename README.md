# react-simplemde-v1
React component wrap for SimpleMDE Markdown Editor(v1.x)


## Installation

```
$ npm install --save react-simplemde-v1
```


## Usage

``` javascript
import ISimpleMDE from 'react-simplemde-v1';

const option = {};

const onReady = function(instance) {
    console.log(instance.value());
};

const onEvents = {
    'change': function() {
        // the 'this' variable can get SimpleMDE instance
        console.log(this.value());
    }
};

return (
    <ISimpleMDE option={option} text={'Hello World!!!'} onReady={onReady} onEvents={onEvents} />
);
```


## propTypes

``` javascript
    className:  React.PropTypes.string,
    style:      React.PropTypes.object,
    option:     React.PropTypes.object.isRequired,
    onReady:    React.PropTypes.func,
    text:       React.PropTypes.string,
    onEvents:   React.PropTypes.object
```

[Read More](https://github.com/NextStepWebs/simplemde-markdown-editor)


## defaultProps

``` javascript
    className: 'react-simplemde',
    style: { width: '100%', height: '100%' },
    onReady: function(instance) {},
    text: '',
    onEvents: {}
```


# License

MIT
