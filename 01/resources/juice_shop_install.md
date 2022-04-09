## Juice Shop Docker image installation

You need to have Docker installed to run Juice Shop as a container inside it. Following the instructions below will download the current stable version (built from master branch on GitHub) which internally runs the application on the currently recommended Node.js version 16.x.

1. Have Docker installed on your computer.

2. On the command line run ```docker pull bkimminich/juice-shop``` to download the latest image described above.

3. Run ```docker run -d -p 3000:3000 bkimminich/juice-shop``` to launch the container with that image.

4. Browse to ```http://localhost:3000```.

*If you are using Docker on Windows - inside a VirtualBox VM - make sure that you also enable port forwarding from host 127.0.0.1:3000 to 0.0.0.0:3000 for TCP.

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [GitHub]: <https://github.com/juice-shop/juice-shop/releases/latest>