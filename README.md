# 404 Page for Web Server Task  

This repository contains a custom **404 error page** designed for use with web servers.  

## Usage  

1. Deploy `404.html` on your web server.
2. To test the error page, visit your website and append a non-existent page name to the URL, e.g.:
   https://yourwebsite.com/random-page
   
   If configured correctly, this should display the custom 404 page.
   
3. For **Nginx**, configure it by adding this to your server block:  

   ```nginx
   error_page 404 /404.html;
   location = /404.html {
       root /usr/share/nginx/html;
       internal;
   }

## Notes
* Ensure `404.html` is placed in the correct directory on your server.
* If using GitHub Pages, the `README.md` will be displayed unless an `index.html` exists.

© 2024, Web Server Task
