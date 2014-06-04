# bs4wp_s

**This is experimental:** Browser-Sync for WordPress Theme Development ~ underscores child theme.

## Usage

Copy files to your theme directory(/wp-content/themes) and move to 'underscores-child' directory. 

Install dependencies. 

	npm install

Postinstall script will clone the '[Automattic/_s](https://github.com/automattic/_s)' theme at parent 'underscores' directory.

Open 'bs-config.js' and 'style.css', set up environment options and edit your theme-name. &rarr; [Child Themes « WordPress Codex](http://codex.wordpress.org/Child_Themes)

Start Browser-Sync

	npm start

Copy 'footer.php' file to child-theme directory, And copy the JavaScript code snippet into 'footer.php'.

It shows on your terminal window. Like this.

> &lt;script type='text/javascript'&gt;//&lt;![CDATA[
;document.write(&quot;&lt;script defer src='//HOST:3000/socket.io/socket.io.js'&gt;&lt;\/script&gt;&lt;script defer src='//HOST:3001/client/browser-sync-client.0.9.1.js'&gt;&lt;\/script&gt;&quot;.replace(/HOST/g, location.hostname));
//]]&gt;&lt;/script&gt;


---

Browser-Sync detect your file changes.
