## Local installation

To run the Juice Shop locally you need to have Node.js installed on your computer. The Juice Shop officially runs on versions 12.x, 14.x, 16.x and 17.x of Node.js, closely following the official Node.js Long-term Support Release Schedule. During development and Continuous Integration (CI) the application is automatically tested with these current versions of Node.js. The officially recommended version to run Juice Shop is either the most recent Long-term Support (LTS) version or the Current Release version. Therefore Juice Shop recommends Node.js 16.x for its own v13.3.0 release.

## From sources

Install Node.js on your computer.

On the command line run ```git clone https://github.com/juice-shop/juice-shop.git --depth 1```.

Go into the cloned folder with ```cd juice-shop```

Run ```npm install```. This only has to be done before the first start or after you changed the source code.

Run ```npm start``` to launch the application.

Browse to ```http://localhost:3000```

## From pre-packaged distribution

Install a 64bit Node.js on your Windows, MacOS or Linux machine.

Download *juice-shop-<version>_<node-version>_<os>_x64.zip* (or .tgz) attached to the latest release on [GitHub].

Unpack the archive and run ```npm start``` in unpacked folder to launch the application

Browse to ```http://localhost:3000```

## Docker image

You need to have Docker installed to run Juice Shop as a container inside it. Following the instructions below will download the current stable version (built from master branch on GitHub) which internally runs the application on the currently recommended Node.js version 16.x.

Install Docker on your computer.
On the command line run ```docker pull bkimminich/juice-shop``` to download the latest image described above.

Run ```docker run -d -p 3000:3000 bkimminich/juice-shop``` to launch the container with that image.

Browse to ```http://localhost:3000```.

If you are using Docker on Windows - inside a VirtualBox VM - make sure that you also enable port forwarding from host 127.0.0.1:3000 to 0.0.0.0:3000 for TCP.

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [GitHub]: <https://github.com/juice-shop/juice-shop/releases/latest>