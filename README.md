lmms.io
======

This repo contains the source for LMMS's new WIP website located at http://lmms.io.

## How to test the website locally ##

1. Clone the code

	```
	$ git clone https://github.com/LMMS/lmms.io.git
	$ cd lmms.io
	```

2. Get Composer

	This project uses [Composer](http://getcomposer.org) for dependency management. You'll have to fetch those dependencies using composer. For this, you must have Composer installed on your system. For quickly installing Composer locally on *nix, run:
	
	```
	$ curl -sS https://getcomposer.org/installer | php
	```
	
	For instructions for other OSs or for installing globally, visit Composer's [Getting Started](https://getcomposer.org/doc/00-intro.md) document.
   
3. Fetch dependencies using composer

	When you downloaded composer locally using the instructions above, fetch the dependencies by running
   
	```
	$ php composer.phar install
	```
   
	You'll have to run this comand every time the dependencies in `composer.json` change.
   
4. Start local server

	Start a local PHP server by running
	
	```
	$ php -S localhost:8000 -t ./
	```
	
	You can then open http://localhost:8000/ in a browser.