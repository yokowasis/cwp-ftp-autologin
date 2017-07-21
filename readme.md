# Auto Login FTP File Manager, Custom CWP Module
Centos Web Panel Custom Module For Auto Login to FTP File Manager

## How to install 
Edit this file (if the file doesn't exist, create it)

    /usr/local/cwpsrv/htdocs/resources/client/include/3rdparty.php
    
add this line

    <li><a href="index.php?module=ftp" target="_BLANK"><span class="icon16 icomoon-icon-arrow-right-3"></span>FTP File Manager</a></li>

Download `ftp.php`
Upload `ftp.php` in `/usr/local/cwpsrv/htdocs/resources/client/modules/`

You can access the module from `Other` Menu in CWP Menu

I am open to suggestion, feel free to pull request if you think you can improve my code.

-------

Optional :
If you want to change the default LINK on CWP FTP File Manager add this lines in `3rdparty.php`

-------

```
<script type="text/javascript">
	jQuery(document).ready(function($) {
		$('a:contains("FTP File Manager")').prop({
			href: 'index.php?module=ftp'
		})
	});
</script>
```
