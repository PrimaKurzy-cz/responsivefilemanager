# Responsive FileManager for TinyMCE and CKEditor

Library Is For Educational Purposes Only

# Original creator

https://github.com/trippo/ResponsiveFilemanager

## 1. Installation:

The easiest way to install the library is using [Composer](https://getcomposer.org/):

```sh
composer require primakurzy/responsivefilemanager
```


## 2. Loading:

Use the following javascript code

```javascript
<script type="text/javascript">
	tinymce.init({
		selector: '#selector',
		external_plugins: {
			'responsivefilemanager': '<?php echo dirname($_SERVER['PHP_SELF']); ?>/vendor/primakurzy/responsivefilemanager/tinymce/plugins/responsivefilemanager/plugin.min.js',
			'filemanager': '<?php echo dirname($_SERVER['PHP_SELF']); ?>/vendor/primakurzy/responsivefilemanager/tinymce/plugins/filemanager/plugin.min.js',
		},
		external_filemanager_path: "<?php echo dirname($_SERVER['PHP_SELF']); ?>/vendor/primakurzy/responsivefilemanager/filemanager/",
		filemanager_title: "File manager",
	});
</script>
```
