# Hugo Frühling Theme

This [Hugo](https://gohugo.io/) theme has been developed for the [Romka!eu](https://romka.eu/en) blog, [where you can find](https://github.com/romka/romka/) a comprehensive demo showcasing the usage of this theme.

The theme utilizes the following JavaScript libraries:
- [lightgallery](https://www.lightgalleryjs.com/),
- [mansory](https://masonry.desandro.com/),
- [swiper](https://swiperjs.com/).

Lightgallery is a paid library. To use it legitimately, you should purchase it and insert your license key into the configuration:
```
[lightgallery]
    licenseKey = 'your-license-key'
```

## Features
The Frühling theme defines four post types:
- two text-based types: _blog_ and _note_,
- and to photo-based types: _gallery_ and _story_.

Each of the content types has a distinct template: blogs and galleries are designed to be more extensive than their counterparts --- notes and stories.

In addition to custom post templates, the theme introduces several shortcodes:

- two types of galleries that can be embedded into a post: `embedded-gallery` and `embedded-local-gallery`. Galleries may contain both photos and videos,
- several custom shortcodes for images,
- the `{{< more >}}` shortcode, which inserts a div with the id `#read-more`, enabling users to navigate from the "read more" link to a custom position on a page.

For more details on available shortcodes, please refer to the `layouts/shortcodes` directory.

The theme is designed for users with a substantial number of photos to post. In the header, the theme displays a _photomosaic_ block --- a row with random photos aggregated from all the photos available under the `content` directory. Each page may have its own photomosaic, but by default, for performance reasons, the number of generated photomosaics is limited, and this can be adjusted in the configuration file:
```
[photomosaic]
    numberOfUniqueMosaics = 25
```