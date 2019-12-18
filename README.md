# @ionic/node-pty-prebuilt

Parallel fork of [`node-pty`](https://github.com/microsoft/node-pty) that prebuilds binaries using Github Actions.

## Contributing

- Prefer upstream fixes
- Try not to modify files other than `README.md` and `.github/workflows/prebuild.yml`
- Configure prebuilt versions in `.github/workflows/prebuild.yml`

### Releasing

1. Pull `master` from [`microsoft/node-pty`](https://github.com/microsoft/node-pty) into `master` branch
1. Merge tagged release commits (e.g. [`0.9.0`](https://github.com/microsoft/node-pty/releases/tag/0.9.0)) into `prebuild` branch
    - Discard any conflicts in `README.md`
1. Push and wait for Github Actions to finish
    - This step creates a release in Github and uploads all the prebuilt binaries.
1. Run `npm publish` to release the new version

## License

Copyright (c) 2012-2015, Christopher Jeffrey (MIT License).<br>
Copyright (c) 2016, Daniel Imms (MIT License).<br>
Copyright (c) 2018, Microsoft Corporation (MIT License).<br>
Copyright (c) 2019, Ionic (MIT License).
