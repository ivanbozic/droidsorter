# Droidsorter
A simple Ruby script to organize a folder of images into their respective `drawable_<dpi>` folders for use on Android.

### How to use
Just symlink the `droidsorter` script into your `usr/local/bin` folder. The usage is pretty straightforward.
- Position yourself into the folder with an export of the images you want to organize. The images should be suffixed with their respective size.
    - e.g. `image@3x` will get moved into the `drawable_xxhdpi` and `image@1,5x` will get moved into the `drawable_hdpi` folder.
- Once you're positioned in the folder, just run `droidsorter` and that's it.
    - Note #1: The images will lose their suffix once they are positioned in the folder.
    - Note #2: Android requires you to name your files using underscores. If your filename contains dashes, Droidsorter will replace them with underscores (e.g. `toolbar-filter-icon.png` will turn into `toolbar_filter_icon.png`).