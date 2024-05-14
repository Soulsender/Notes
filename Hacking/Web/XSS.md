### XSS DOM
- You can break out from HTML input
- If input is filtered, you can use errors with `onerror`
### XSS Reflected
- If input is filtered, try capitalizing it instead
### XSS Stored
- If input has min/max restriction, you can edit HTML and change it client-side
### Changing Cookies with JavaScript
- Cookie has to have HttpOnly unchecked
- RENAVIGATE to root of website, reloading page will not work