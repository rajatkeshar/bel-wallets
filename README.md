# Belrium Wallet
##### (Belrium Nano fork)

[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)

## Development

```
git clone https://github.com/rajatkeshar/bel-wallets.git
cd bel-wallets
npm install
npm run dev
```

Open https://localhost:8080

For ease of development, you can setItem in localStorage to prefill a passphrase, e.g.:
```
localStorage.setItem('passphrase', 'wagon stock borrow episode laundry kitten salute link globe zero feed marble')
```

And then you can setItem in localStorage to login automatically
```
localStorage.setItem('autologin', true)
```

## Build

```
npm run build
```

## Electron

### Start


Start the Electron client. Before staring you need to make sure the application is built. If you need to built the entire application, run

```
npm run build
```

as mentioned before. And if you want to solely build electron app, run

```
npm run build-electron
```

Then, in order to launch electron, you can run

```
npm run start
```

### Windows

Build package for Windows (on Windows in [Git BASH](https://git-for-windows.github.io/)).

```
npm run pack:win
```

### macOS

Build package for macOS (on macOs)

```
npm run pack
```

### Linux

Build package for Linux (on Linux).

```
npm run pack
```

## Run unit tests

### Single run
```
npm run test
```

### Run each time a file changes
```
npm run test-live
```

## Run end-to-end tests

### Setup

Setup protractor

```
./node_modules/protractor/bin/webdriver-manager update
```

Setup a lisk test node to run on localhost:4000 as described in https://github.com/LiskHQ/lisk#tests

And run it with [pm2](http://pm2.keymetrics.io/).

### Run

Start the development version of liskish-wallet:

```
npm run dev
```

Run the protractor tests (replace `~/git/lisk/` with your path to lisk core):

```
./e2e-test-setup.sh ~/git/lisk/
npm run e2e-test
```

## Launch React Storybook

To launch storybook sandbox with components run
```
npm run storybook
```
and go to

http://localhost:6006/



## Authors

- Matteo Ferrari (hirish) <matteo.ferrari@sapiensproject.io>
- Ricardo Ferro <ricardo.ferro@gmail.com>
- Oliver Beddows <oliver@lightcurve.io>
- V??t Stanislav <vit@lightcurve.io>
- Tobias Schwarz <tobias@lightcurve.io>
- Ali Haghighatkhah <ali@lightcurve.io>
- Yashar Ayari <darkyashi@gmail.com>

## License

Copyright ?? 2018 Matteo Ferrari
Copyright ?? 2016-2017 Lisk Foundation

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the [GNU General Public License](https://github.com/hirishh/liskish-wallet/tree/master/LICENSE) along with this program.  If not, see <http://www.gnu.org/licenses/>.

***

This program also incorporates work previously released with lisk-nano `0.1.2` (and earlier) versions under the [MIT License](https://opensource.org/licenses/MIT). To comply with the requirements of that license, the following permission notice, applicable to those parts of the code only, is included below:

Copyright ?? 2016-2017 Lisk Foundation
Copyright ?? 2015 Crypti

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
