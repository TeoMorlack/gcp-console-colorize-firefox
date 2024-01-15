gcp-console-colorize
===

Foxfied fork of Chrome extension for changing header color for GCP console, which is made by [yfuruyama](https://github.com/yfuruyama).

e.g. Change header color to red for a production project.

![screenshot](./image/gcp-console-colorize.png)

## Create XPI

1. Get the credentials from AMO.

2. Download NodeJs and install web-ext

```
npm install --global web-ext
```

3. From repo directory run

```
web-ext sign --api-key="JWT issuer" --api-secret="JWT secret"
```

4. Rename the extension generated inside [web-ext-artifacts](./web-ext-artifacts/) accordingly

```
mv ./web-ext-artifacts/*.xpi ./web-ext-artifacts/gcp-console-colorize-$VERSION.xpi
```

5. Install the xpi from your `about:addons` page

## See Also

* [original repo](https://github.com/yfuruyama/gcp-console-colorize)
