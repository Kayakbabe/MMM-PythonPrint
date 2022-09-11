# MMM-PythonPrint

doc for [MMM-PythonPrint](https://github.com/sdetweil/MMM-PythonPrint)

## Install:

* Clone this modules URL from github

* Edit `config.js` and add a block like this:

	```js
	{
		module:"MMM-PythonPrint",
		position:"center",
		disabled:false,
		config: {
			// name of the python process to execute (could be python3)
			pythonName: 'python',
			// command file in module folder
			// if false, YOU will provide the full path to the python program
			localfolder: true,

			// spawn a python pgm that writes over and over (timed maybe), but keeps running
			command: 'printit.py',
			script_is_long_running: true,

			// spawn a one time output  script, but relaunch it every cycletime milliseconds
			// script_is_long_running: false,
			// command: 'printitonce.py',
			cycletime: 2000,

			// print debugging messages from the node_helper
			debug: true
		}
	}
	```

## Styling

The class `PythonPrint` is added to the css.

To change the color of the print, add to `custom.css`:

```css
.MMM-PythonPrint .PythonPrint {
	color: red;
}
```
