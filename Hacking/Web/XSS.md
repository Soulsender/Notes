### XSS DOM
![[Pasted image 20221219000148.png]]
![[Pasted image 20221219000225.png]]

- You can break out from HTML input
![[Pasted image 20221219000323.png]]

- If input is filtered, you can use errors with `onerror`
![[Pasted image 20221219000653.png]]
---
### XSS Reflected
![[Pasted image 20221219000950.png]]

- If input is filtered, try capitalizing it instead
![[Pasted image 20221219001144.png]]
---
### XSS Stored
![[Pasted image 20221219001314.png]]
- If input has min/max restriction, you can edit HTML and change it client-side
---
### Changing Cookies with JavaScript

![[Pasted image 20221219001804.png]]
- Cookie has to have HttpOnly unchecked

![[Pasted image 20221219002037.png]]
![[Pasted image 20221219002109.png]]
![[Pasted image 20221219002209.png]]
- RENAVIGATE to root of website, reloading page will not work