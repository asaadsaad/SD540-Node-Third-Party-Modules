### SD540-Node-Third-Party-Modules
In a new TS project (using `ts-node`):
* Create a folder `/input` and place 10 high-resolution photos from [Pexels](https://www.pexels.com/).
* Create an empty folder `/output`.
* Read Node documentation to learn about [working with folders in Node](https://nodejs.org/en/learn/manipulating-files/working-with-folders-in-nodejs) using the `fs` core module.
* Write a script read the images' name in both the `/input` and `/output` folders, and determine the difference between them (files that exist in `/input` but does not exist in `/output`).
* If an image exists in `/input` and does not exist in `/output`, use [Sharp](https://www.npmjs.com/package/sharp) to resize the source image to a thumbnail size of 200 width, and save the thumbnail image in the `/output` directoty.
* Use [Node Cron](https://www.npmjs.com/package/node-cron) to schedule a cron job using the following step value `*/30 * * * * *` that runs your script every 30 seconds.
  
Remember to install the definately typed (DT) package as a development dependency if the package does not provide types.
