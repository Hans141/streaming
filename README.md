## streaming

### 0. Checkout master
`git checkout master`
### 1. Install package dependencies
`npm install` or `yarn`
### 2. Run the node server
`node index.js`
### 3. Run ffmpeg
`ffmpeg -f v4l2 -framerate 20 -video_size 640x480 -i /dev/video0 -f mpegts -codec:v mpeg1video -s 640x480 -b:v 600k -bf 0 http://localhost:8080/mystream`
### 4. Check [localhost:8080](http://localhost:8080)

