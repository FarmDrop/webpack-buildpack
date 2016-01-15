# Webpack Heroku buildpack

This is a small buildpack to get the `webpack:compile` rake task from the
[webpack-rails gem](https://github.com/mipearson/webpack-rails) to happen
as part of the Heroku deploy process.

## Usage

Enable the [Heroku buildbpack multi](https://github.com/ddollar/heroku-buildpack-multi)
and then add `https://github.com/FarmDrop/webpack-buildpack` to your `.buildpacks`
file.

The buildpack will only apply itself if it detect a `Gemfile` containing the
`webpack-rails` gem