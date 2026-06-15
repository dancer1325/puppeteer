# Puppeteer

![](https://user-images.githubusercontent.com/10379601/29446482-04f7036a-841f-11e7-9872-91d1fc2ea683.png)

* Puppeteer
  * == JavaScript library
    * allows
      * control Chrome OR Firefox, -- via --
        * [DevTools Protocol](https://chromedevtools.github.io/devtools-protocol/)
          * default -- for -- automating Chrome
        * [WebDriver BiDi](https://pptr.dev/webdriver-bidi)
          * default -- for -- automating Firefox
    * provides
      * HIGH-level API / abstract
        * DevTools Protocol
        * WebDriver BiDi
    * by default,
      * runs headless (== NO UI)

## documentation

* [here](docs/)

## MCP

* [`chrome-devtools-mcp`](https://github.com/ChromeDevTools/chrome-devtools-mcp)
  * == Puppeteer-based MCP server -- for -- browser automation & debugging
* [WebMCP](https://pptr.dev/guides/webmcp) API
