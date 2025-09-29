# futurium-suitcase-reinforcement-learning-2
Reinforcement Learning 2 as a suitcase exhibit for Futurium

This variant of the original exhibit splits the functionality over two screens. It's designed
for two iPads with 2360-by-1640-pixel resolution at 264 ppi (1180x820 logical resolution). 
One in landscape orientation, the other in portrait.

## Building

Requires Node.js (v18.19 or greater) and npm.

Run the following from the root directory of the project:

```bash
npm install
npm run build
```

This will create a `dist` directory with the compiled exhibit. This directory can be served by any web server.

## Development

Run both

```bash
npm run watch:copy
```

and

```bash
npm run watch:compile
```

The first will copy any files changed in `extras` to `dist` (without requiring a full build), and
the second will recompile the JavaScript and SASS files (it actually runs watch on the inner
project, inside of `dist`).

## Configuration

The config directory has several data definitions.

You can override any of them in the settings-exhbit.yml file in the root of the built project.

## Running

Open `station-1.html` and `station-2.html` in two separate iPads.

## Sentry

The app supports Sentry.

The `index.html` page can take the DSN from the `sentry-dsn` query string parameter.

It can also get the DSN from the `app.sentry.dsn` configuration key in the  `settings.yml` file.

## Credits

This adaptation was developed by Eric Londaits for Imaginary gGmbH.

Supported by [Futurium](http://futurium.de/).

## License

Code licensed under the MIT License. See [LICENSE](LICENSE) for details.

Copyright 2025 Imaginary gGmbH.
