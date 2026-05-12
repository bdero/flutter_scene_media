# flutter_scene_media

Image assets used by the [`flutter_scene`](https://github.com/bdero/flutter_scene)
README: the project logo and the demo animations.

They live in their own repository so the large source files don't
inflate `flutter_scene`'s git history or clone size. The `flutter_scene`
README references them via
`https://raw.githubusercontent.com/bdero/flutter_scene_media/main/<file>`.

| File | Used for |
| --- | --- |
| `DashColorTransparent.svg` | Header logo |
| `dashgameported2.webp` | Game demo |
| `hexagons3.webp` | Procedural geometry demo |
| `DamagedHelmet.webp` | glTF / PBR demo |
| `car_example.webp` | Animated example app |
| `cloning.webp` | Node cloning demo |

The `.webp` files are animated WebP, downscaled to 720px wide with the
original frame rate preserved, lossy-encoded with `gif2webp`. The
original full-resolution GIF exports (`dashgameported2.gif`, etc.) are
kept in this repo as archival sources. The README points at the WebP
versions because they serve with an `image/webp` content type
(`raw.githubusercontent.com` serves multi-megabyte GIFs as
`application/octet-stream`, which neither browsers with `nosniff` nor
pub.dev's image proxy will render as an image).
