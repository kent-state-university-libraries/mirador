# Mirador

Omeka plugin to display TIFF images in Mirador IIIF viewer

## Install

1. Install IIIF Image Server
  * At Kent State University Libraries we used [Loris on RHEL 7](https://github.com/loris-imageserver/loris/blob/development/doc/redhat-7-install.md)
2. You'll want to be sure to configure your IIIF resolver to serve files from your Omeka "files/original" folder.
  * You can either set your resolver's source image root to be the "files/original" folder, or you can create a new folder on your server and use a symlink to point it to "files/original"
3. Clone this repository in your Omeka "plugins" folder `git clone https://github.com/kent-state-university-libraries/Mirador.git`
4. Build mirador
  * `cd Mirador`
  * `git submodule init views/public/mirador`
  * `cd views/public/mirador`
  * follow the [build instructions for Mirador](https://github.com/ProjectMirador/mirador)
5. Enable the plugin and complete the configuration form
6. All your TIFF files should now be displayed using the Mirador viewer on the public display