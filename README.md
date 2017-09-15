## corgi-theme

This repo is the UI style for [corgi-react](https://github.com/HenryYong/corgi-react).



### Install

```javascript
npm install corgi-theme --save
```



### Usage

In `main.js`:

```javascript
import 'corgi-theme'
```

Also, please make sure you have correct setting for files of font icons. Add follow setting in `webpack.config.js`:

```javascript
module: [
    loaders: {
    	{
  			test: /\.(eot|woff|ttf|svg)$/,
             loader: 'file-loader'
        }
  	}
]
```



Meanwhile, it supports load on demand. For example:

```javascript
import '{your-path}/node_modules/corgi-theme/dist/Button.css'
import '{your-path}/node_modules/corgi-theme/dist/Checkbox.css'
```



### Custom Compiling

You can modify files in following path: `corgi-theme/src`, and use gulp (I am using `gulp` and `gulp-sass` which can be found in `package.json`) to compile them.