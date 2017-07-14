# Heroku Optimizers Buildpack

Add binaries for image optimization on Heroku.

Binaries in this buildpacks :

- `advpng`
- `gifsicle`
- `jpegoptim`
- `jpegtran`
- `optipng`
- `pngcrush`
- `pngquant`

Binaries are in this git repo in `vendor/optimizers/`

On compilation :

- Binaries are copied into vendor/optimizers
- Symlink to binaries is added to ensure next buildpacks will have binaries available
- vendor/optimizers is added to PATH through a .profile.d script
- Version of each binaries is displayed


