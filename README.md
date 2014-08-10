polymer_docs_nginx
==================
中文readme:[readme](README_ZH.md)
## requirements:

- To compile the doc , you need all things that [polymer/docs] (https://github.com/Polymer/docs/) needed except App Engine SDK.

- To browse the doc , you need compiled dirs : `/_site` , `/components` . This not include designer and apps.

- To publish as a website , you need compiled dirs : `/_site` , `/polymer-all/projects` , `/components`

## site setting for nginx

- see `docs_site.nginx`

## Usage:

1. add `docs_site.nginx` to your `sites-available` dir or nginx.conf

2. replace $polymer_docs_root to your docs path.

3. set the permission to allow nginx read the file

4. replace 40000 to the port you want.

5. reload or restart your nginx

