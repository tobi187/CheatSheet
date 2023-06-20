
# Best Practices

**Keine Inline Scripts(JS) oder Styles (CSS benutzen)**
	-> In Verbindung mit CSP

# Header

Zu viel aussagende Header (zb verwendetes Framework + Version) vermeiden

### Http Security Header 

| Name | Prefered Value |
| -------|--------------|
| [HSTS](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Strict-Transport-Security) | idk |
| [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options?retiredLocale=de) | deny |
| [X-Content-Type-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Content-Type-Options) | nosniff |
| [Content-Security-Policy](https://developer.mozilla.org/en-US/docs/Web/HTTP/CSP) | idk |

[Csp-Evaluator](https://csp-evaluator.withgoogle.com/): gutes Tool zum Überprüfen des Content-Security-Policy