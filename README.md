# Puppeteer

![](https://user-images.githubusercontent.com/10379601/29446482-04f7036a-841f-11e7-9872-91d1fc2ea683.png)

* Puppeteer
  * == JavaScript library
    * allows
      * control Chrome OR Firefox, -- via --
        * [DevTools Protocol](https://chromedevtools.github.io/devtools-protocol/)
        * [WebDriver BiDi](https://pptr.dev/webdriver-bidi)
    * provides
      * HIGH-level API
    * by default,
      * runs headless (== NO UI)

## documentation

* [here](docs/index.md)

## Installation

```bash npm2yarn
npm i puppeteer # Downloads compatible Chrome during installation.
npm i puppeteer-core # Alternatively, install as a library, without downloading Chrome.
```

## MCP

* support
  * [`chrome-devtools-mcp`](https://github.com/ChromeDevTools/chrome-devtools-mcp)
    * == Puppeteer-based MCP server -- for -- browser automation & debugging
  * [WebMCP](https://pptr.dev/guides/webmcp) API
