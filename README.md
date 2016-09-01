# ES2015-Demo
ES2015 Demo

# Demo can be run in two ways

1) Directly with Chrome console
2) Install node in the machine - https://nodejs.org/en/
3) With any transpilers like Babel
	1) Install Babel with NPM Package
		a) npm install babel-cli
		b) npm install babel-preset-es2015
	2) create .babelrc file with the following content
			{
				"presetS" : ["ES2015"]
			}
	3) Create a src directory and with content in src.js and create an empty directory called dest & a file dest\main.js
	4) Use the following npm commands 
			a) Add the following compile commands in package.json 
			   "scripts": {
					"build": "babel src -d dest"
				},
				"scripts" : {
					"build": "babel --presets es2015 src -d dest"
				}
			b) from the project path -> npm run build
	5) This should build src/main.js into dest/main.js
	6) Dest/main.js can be run as part of any html file and launched through any editors like VSCode that can run & output a javascript file
