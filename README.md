# Clinton CAT

## About

# EXPERIMENTAL

Chrome Browser Extension for automatically
searching [Rossmann's Consumer Action Taskforce (CAT)](https://wiki.rossmanngroup.com/wiki/Mission_statement) articles
for the current page being visited.

## Operation

If a CAT wiki page for the website is found then the plugin toolbar icon will indicate the number of controversies found.
You might also see a clickable angry cat image in the page.

## Install

As this is not yet on the Chrome Web Store it's necessary to download and manually install it.

For Chrome:

1. Download a [release](https://github.com/WayneKeenan/ClintonCAT/releases) .
2. Open Extension settings: e.g. `chrome://extensions/`  or `brave://extensions/` etc.
3. Enable Developer Mode
4. Click `Load Unpacked`
5. Navigate to the unzipped folder.


For Firefox:

1. Open: about:debugging#/runtime/this-firefox
2. Expand 'Temporary Extenstions'
3. Click 'Load Temporary Add-on...'
4. Navigate to the unzipped folder and open `manifest.json`

# Developer

## Checkout and build the extension:

```shell
git checkout git@github.com:WayneKeenan/ClintonCAT.git
cd ClintonCAT
npm install
npm run build:chromium    # Chrome
# or
npm run build:gecko       # Firefox 
```

The compiled extension will be output in the `dist` folder.

## Testing

### Automated unit, integration and browser testing

```shell
npm test
```

### Manual testing using local http server

```shell
npx http-server tests/www 

# install using: npm install --global http-server
```

# Contributions

Thanks to contributions from the following people that I added outside of a PR:

- @blimeybloke  (Settings and whitelisting)
- @lnardon (Firefox)
- @khonkhortisan (Firefox)
- @SalimOfShadow (Multiple tab prevention)
- @EricFrancis12 (Toggle on/off)

# Attributions

- [Icons on the html test page by Gatoon Team](https://www.iconarchive.com/show/gartoon-devices-icons-by-gartoon-team.html)

