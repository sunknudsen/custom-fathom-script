# Custom Fathom script

## Custom implementation of [Fathom](https://usefathom.com/) [script](https://cdn.usefathom.com/script.js) used to self-host [privacy-conscious](https://usefathom.com/privacy-focused-web-analytics) tracker.

**Why do I self-host tracker?** I am uncomfortable allowing any third-party (including trusted ones such as Fathom) into my JavaScript environments which could be used as a backdoor.

**This projects solves two problems…**

First, code is deobfuscated so one can audit how it works.

Second, it adds a `data-domain` attribute so one can set [custom domain](https://usefathom.com/docs/script/custom-domains) which, in [reference implementation](https://usefathom.com/docs/script/embed), is set to hostname of script.

```html
<script
  src="script.min.js"
  data-domain="twenty-graceful.sunknudsen.com"
  data-site="JNIACVCL"
  …
></script>
```
