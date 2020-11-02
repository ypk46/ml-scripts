## ML Scripts

A personal compilation of useful scripts when working on ML projects.

### Pascal VOC to YOLO

Script: `pascal_voc_to_yolo.py`

**How to use it?**

1. Move your images and xml files to a new directory in the root of the project. Example: `data/train` and `data/test` where all your train images/xml files would be inside the `data/train` and same for any other directory.
2. Update the `dirs` array (line 8) with the relative path of the directories created on step 1.
3. Update the `classes` array line (line 9) with your list of classes/labels.
4. Run the script. Upon running all the required files to train your YOLO model should be inside the `output` directory.

**Notes**:

- You can change the output directory by changing the line 7.
- All your images will be copied to the output directory, be sure to clean it up after using. (I chose this approach so you can take the output directory as it is.)
- Your list `txt` files will probably required the path to be updated if you are planning to training on another computer (or cloud instance). Make sure to replace everything before the `/output` segment of the path with the absolute path where you are planning to place your files on your training machine.

_Disclaimer: This code is a modified version of [Amir22010's gist](https://gist.github.com/Amir22010/a99f18ca19112bc7db0872a36a03a1ec)._

### Upcoming Changes

- [ ] Add flag/params to customize the behavior without modifying scripts.
- [ ] Implement is as a CLI tool (maybe).
- [ ] Add more scripts...
