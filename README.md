# Mailing lists

Mailchimp mailing list templates

## the old skool way

1. Edit HTML and preview in your browser
2. Copy HTML into Mailchimp 'code your own' template editor
3. test test test...

## the hip way

Using [MJML](https://mjml.io/)

1. watch and convert `mjml` to `html` using e.g.:
```
    mjml -w ./kunsthalle.mjml -o kunsthalle.html   
```
2. Reload `kunsthalle.html` in your browser ~~manually~~ automagically e.g. with [`browser-sync`](https://www.browsersync.io/):
```
    browser-sync start --server --files ./kunsthalle.html 
```
3. Edit `mjml`
4. When template is coded, copy generated HTML to a separate file and add mailchimp specific attributes like `mc:edit` and `mc:repeatable`
