# Artwork

Icons and other artwork used in [helloSystem](https://hellosystem.github.io/).

* `elementary-hello` holds icons specifically designed for helloDesktop. For conceptual human interface guidelines regarding helloSystem, please loosely refer to [ISBN 978-0-201-2216-4](https://dl.acm.org/doi/book/10.5555/573097). __Important:__ The objective is not to create a visual replica, but to apply the published concepts in a way that makes users experienced in those metaphors feel instantly "at home".

* `elementary-xfce` was imported from [xubuntu-artwork_16.04.2.tar.xz](http://archive.ubuntu.com/ubuntu/pool/universe/x/xubuntu-artwork/xubuntu-artwork_16.04.2.tar.xz) and is mirrored here. Its contents are used as a fallback for icons which do not exist in `elementary-hello`. __Do not make changes here.__ These files are merely provided as a convenience mirror here. For visual design guidelines regarding the elementary-xfce visual style, please refer to [shimmerproject/elementary-xfce](https://github.com/shimmerproject/elementary-xfce/).


## Contributing

Please look up the location of an icon in `elementary-xfce`, then create an icon in the corresponding location in `elementary-hello`. When contributing icons, please also add a `.svg` in the `scalable` directory next to the various sizes of `.png` files.

To quickly find the name for an icon (not its various symlinks), use something like

```
find ./elementary-xfce -type l -name '*trash*' -exec ls -lh {} \; | cut -d ">" -f 2 | sort | uniq
(...)
 user-trash-full.png
 user-trash.png
```
