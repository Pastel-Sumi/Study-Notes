* We use optional parameters for backward compatibility
* All types of API will have a type of versioning
![[Pasted image 20260922183339.png]]
"GET is only for reading, we shouldn't create anything."
Check public APIs to learn about documentations and good practices that popular sites use (Ex: Twitter, Stripe, etc).
* Always remember optional parameters and make good use of GET/POST etc.
![[Pasted image 20260922184854.png]]
* We want things to be backwards compatible.
* We want endpoints to be clearly defined.
* You don't want endpoints to conflict with each other.
* You want to provide pagination (limit and offset).
* 