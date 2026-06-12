---
sidebar_label: Configuration
---

# Configuration interface

Defines options to configure Puppeteer's behavior during installation and runtime.

See individual properties for more information.

### Signature

```typescript
export interface Configuration
```

## Properties

| Property | Modifiers | Type | Description | Default |
| -------- | --------- | ---- | ----------- | ------- |
| <span id="_chrome-headless-shell_">"chrome-headless-shell"</span> | `optional` | [ChromeHeadlessShellSettings](./puppeteer.chromeheadlessshellsettings.md) | | |
| <span id="cachedirectory">cacheDirectory</span> | `optional` | string | Defines the directory to be used by Puppeteer for caching. Can be overridden by `PUPPETEER_CACHE_DIR`. | `path.join(os.homedir(), '.cache', 'puppeteer')` |
| <span id="chrome">chrome</span> | `optional` | [ChromeSettings](./puppeteer.chromesettings.md) | | |
| <span id="defaultbrowser">defaultBrowser</span> | `optional` | [SupportedBrowser](./puppeteer.supportedbrowser.md) | Specifies which browser you'd like Puppeteer to use. Can be overridden by `PUPPETEER_BROWSER`. | `chrome` |
| <span id="executablepath">executablePath</span> | `optional` | string | Specifies an executable path to be used in [puppeteer.launch](./puppeteer.puppeteernode.launch.md). Can be overridden by `PUPPETEER_EXECUTABLE_PATH`. | **Auto-computed.** |
| <span id="experiments">experiments</span> | `optional` | [ExperimentsConfiguration](./puppeteer.experimentsconfiguration.md) | Defines experimental options for Puppeteer. | |
| <span id="firefox">firefox</span> | `optional` | [FirefoxSettings](./puppeteer.firefoxsettings.md) | | |
| <span id="loglevel">logLevel</span> | `optional` | 'silent' \| 'error' \| 'warn' | Tells Puppeteer to log at the given level. | `warn` |
| <span id="skipdownload">skipDownload</span> | `optional` | boolean | Tells Puppeteer to not download during installation. Can be overridden by `PUPPETEER_SKIP_DOWNLOAD`. | |
| <span id="temporarydirectory">temporaryDirectory</span> | `optional` | string | Defines the directory to be used by Puppeteer for creating temporary files. Can be overridden by `PUPPETEER_TMP_DIR`. | `os.tmpdir()` |
