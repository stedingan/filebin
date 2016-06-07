# FileBin

A pastebin software running on [https://paste.xinu.at](https///paste.xinu.at).
In addition to uploading text and code it also supports binary files.

Additional documentation can be found in [`./doc`](doc/).

## Installation/Development

Git is used for tracking changes and updating installations. The repository is
located at [https://git.server-speed.net/users/flo/filebin/](https///git.server-speed.net/users/flo/filebin/).
Clone the repository and follow the instructions in `./INSTALL`. Do not
install using tarballs as this is not supported.

`dev` is the development branch and should not be used in production. All
stable changes go to `master` and will be tagged regularly following [semver
guidelines](http://semver.org/).

There is currently no bug tracking software.

### Mailing List

Currently there is only [one mailing
list](https///lists.server-speed.net/listinfo/filebin-general) for everything
(general discussion, patches, announcements, ...). If need be more lists will be
created at a later date.

### Patches

Please submit patches (preferably git send-email) to the [filebin-general
mailing list](https///lists.server-speed.net/listinfo/filebin-general). You do
not need to register to be allowed to post.


## Dependencies

*  PHP >=5.5 with the following modules
    * gd for thumbnail generation
    * exif for thumbnail generation
    * phar for tarball creation
    * mysql, mysqli, pgsql, pdo_mysql (any of those) for database access

*  perl with the following CPAN Modules
    * Text::Markdown for markdown rendering

*  [pygmentize](http://pygments.org/) for code highlighting
*  [ansi2html](http://pypi.python.org/pypi/ansi2html) for shell output rendering (ANSI color codes)
*  [qrencode](http://megaui.net/fukuchi/works/qrencode/index.en.html) for qrcode generation
*  [imagemagick](http://www.imagemagick.org/) for additional thumbnail generation
*  [node.js](https///nodejs.org/) for javascript minification

