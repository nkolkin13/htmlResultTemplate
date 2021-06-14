# htmlResultTemplate
simple template for html+javascript to make table of comparison images with toggleable columns

# Usage
Edit variables at the top of base.html based on your needs:

<ul>
  <li>N = number of image rows (each row should be a comparision/ set of inputs and outputs)</li>
  <li>im_folders = array of folder names in ./images/</li>
  <li>im_folder_display_name = displayed column name corresponding to image folder</li>
</ul>

in ./images/:

<ul>
  <li>each folder should contain N images of the same filetype (currently everything is expected to be a '.png' file and this is hardcoded in base.html, but the image loading</li>
  <li>functions in base.html accept an extension, and it should be easy to extend base.html to allow each folder having its own filetype)</li>
</ul>

image filenames should be a zero-padded index between 000.png and 999.png, and images that should go in the same row of the comparison should have the same filename in all folders.
