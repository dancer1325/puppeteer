# `export type ExperimentsConfiguration = Record<string, never>;`
* == Puppeteer's experimental options

---

# `export interface Configuration`
* == options to configure Puppeteer's behavior during installation and runtime

* `cacheDirectory?: string`
  * == directory used by Puppeteer for caching
  * can be overridden by `PUPPETEER_CACHE_DIR`
  * default: `path.join(os.homedir(), '.cache', 'puppeteer')`
* `executablePath?: string`
  * == executable path used in `puppeteer.launch`
  * can be overridden by `PUPPETEER_EXECUTABLE_PATH`
  * default: auto-computed
* `defaultBrowser?: SupportedBrowser`
  * == browser Puppeteer will use
  * can be overridden by `PUPPETEER_BROWSER`
  * default: `chrome`
* `temporaryDirectory?: string`
  * == directory used by Puppeteer for temporary files
  * can be overridden by `PUPPETEER_TMP_DIR`
  * default: `os.tmpdir()`
* `skipDownload?: boolean`
  * == skip browser download during installation
  * can be overridden by `PUPPETEER_SKIP_DOWNLOAD`
* `logLevel?: 'silent' | 'error' | 'warn'`
  * == log level
  * default: `warn`
* `experiments?: ExperimentsConfiguration`
  * == experimental options
* `chrome?: ChromeSettings`
  * == Chrome-specific settings
* `['chrome-headless-shell']?: ChromeHeadlessShellSettings`
  * == Chrome Headless Shell-specific settings
* `firefox?: FirefoxSettings`
  * == Firefox-specific settings

---

# `export interface ChromeSettings`
* == Chrome-specific browser settings

* `skipDownload?: boolean`
  * == skip Chrome download during installation
  * can be overridden by `PUPPETEER_CHROME_SKIP_DOWNLOAD`
  * default: `false`
* `downloadBaseUrl?: string`
  * == URL prefix used to download Chrome
  * must include protocol, must **not** have trailing slash
  * can be overridden by `PUPPETEER_CHROME_DOWNLOAD_BASE_URL`
  * default: `https://storage.googleapis.com/chrome-for-testing-public`
* `version?: string`
  * == Chrome version to use
  * can be overridden by `PUPPETEER_CHROME_VERSION` or `PUPPETEER_SKIP_CHROME_DOWNLOAD`
  * default: pinned version supported by current Puppeteer

---

# `export interface ChromeHeadlessShellSettings`
* == Chrome Headless Shell-specific browser settings

* `skipDownload?: boolean`
  * == skip Chrome Headless Shell download during installation
  * can be overridden by `PUPPETEER_CHROME_HEADLESS_SHELL_SKIP_DOWNLOAD` or `PUPPETEER_SKIP_CHROME_HEADLESS_SHELL_DOWNLOAD`
  * default: `false`
* `downloadBaseUrl?: string`
  * == URL prefix used to download Chrome Headless Shell
  * must include protocol, must **not** have trailing slash
  * can be overridden by `PUPPETEER_CHROME_HEADLESS_SHELL_DOWNLOAD_BASE_URL`
  * default: `https://storage.googleapis.com/chrome-for-testing-public`
* `version?: string`
  * == Chrome Headless Shell version to use
  * can be overridden by `PUPPETEER_CHROME_HEADLESS_SHELL_VERSION`
  * default: pinned version supported by current Puppeteer

---

# `export interface FirefoxSettings`
* == Firefox-specific browser settings

* `skipDownload?: boolean`
  * == skip Firefox download during installation
  * can be overridden by `PUPPETEER_FIREFOX_SKIP_DOWNLOAD`
  * default: `true`
* `downloadBaseUrl?: string`
  * == URL prefix used to download Firefox
  * must include protocol, must **not** have trailing slash
  * can be overridden by `PUPPETEER_FIREFOX_DOWNLOAD_BASE_URL`
  * default: `https://archive.mozilla.org/pub/firefox/releases`
* `version?: string`
  * == Firefox version to use
  * can be overridden by `PUPPETEER_FIREFOX_VERSION`
  * default: pinned version supported by current Puppeteer
