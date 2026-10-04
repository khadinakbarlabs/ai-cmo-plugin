# WordPress through WP-CLI

Primary contracts: https://developer.wordpress.org/cli/commands/post/create/ and https://developer.wordpress.org/cli/commands/post/get/ . Inspected October 5, 2026. Use externally installed WP-CLI on the user's authorized WordPress host. Confirm site, multisite URL, operator rights and installed command help; never inspect or print configuration secrets.

An authorized remote draft can use:

```sh
wp post create ./approved-content.html --post_title='Approved title' --post_status=draft --porcelain
wp post get <returned-id> --fields=ID,post_status,post_title --format=json
```

Resolve installation targeting through the installed `--path`, `--url` or `--ssh` support. Content belongs in a file, not interpolated shell text. Draft creation still writes to an external site and requires an authorized destination. Check the resulting content, slug, metadata, images, accessibility and rendering. A publish request uses the installed post-update contract and separate readback; creating a draft does not publish it.

Do not install themes/plugins, change permissions, overwrite an existing post, or alter the site merely to deliver copy. Use Markdown/HTML exports when server access is unavailable.
