<h1 style="font-family: Roboto" align="center">
HTML META TAGS CHEAT SHEET 
</h1>

<h3 style="font-family: Roboto">
Meta Tags 
</h3>

```html
<meta charset='utf-8'> 

<!-- title -->
<title>···</title>
<meta property='og:title'  content='···'>
<meta name='twitter:title' content='···'>

<!-- url -->
<link rel='canonical'       href='http://···'>
<meta property='og:url'  content='http://···'>
<meta name='twitter:url' content='http://···'>

<!-- description -->
<meta name='description'         content='···'>
<meta property='og:description'  content='···'>
<meta name='twitter:description' content='···'>

<!-- image -->
<meta property="og:image"  content="http://···">
<meta name="twitter:image" content="http://···">

<!-- ua -->
<meta http-equiv='X-UA-Compatible' content='IE=edge,chrome=1'> 

!-- viewport -->
<meta name='viewport' content='width=device-width'>
<meta name='viewport' content='width=1024'> 
```

<h3 style="font-family: Roboto">
More Opengraph 
</h3>

```html
<meta property='og:site_name' content='···'>
<meta property='og:type' content='website'> 

<meta property='fb:app_id' content='···'>
<meta property='fb:admins' content='UID1,UID2'>
<!-- ···unless there's app_id -->

<meta property='og:audio' content='http://···/theme.mp3'>
<meta property='og:video' content='http://···/trailer.swf'> 
``` 

<h3 style="font-family: Roboto">
Apple-only 
</h3>

```html
<meta name='format-detection' content='telephone=no'>
```

<h3 style="font-family: Roboto">
Add to Homescreen 
</h3>

```html
<meta name='mobile-web-app-capable' content='yes'>
<meta name='apple-mobile-web-app-capable' content='yes'> 

<meta name='apple-mobile-web-app-status-bar-style' content='black'>
<!-- black | black-translucent | default --> 
```

<h3 style="font-family: Roboto">
Theme Color 
</h3>

```html
<meta name='theme-color' content='#ff00ff'> 
```

<h3 style="font-family: Roboto">
Icons 
</h3>

```html
<!-- Minimal -->
<link rel='icon' type='image/png' href='favicon@32.png'>
<link rel='icon' sizes='192x192' href='icon@192.png'>
<link rel='apple-touch-icon' href='icon@152.png'>
<meta name='msapplication-square310x310logo' content='icon@310.png'> 

<!-- Apple -->
<link rel='apple-touch-icon' href='touch-icon-iphone.png'>
<link rel='apple-touch-icon' sizes='76x76' href='touch-icon-ipad.png'>
<link rel='apple-touch-icon' sizes='120x120' href='touch-icon-iphone-retina.png'>
<link rel='apple-touch-icon' sizes='152x152' href='touch-icon-ipad-retina.png'> 

!-- Microsoft -->
<meta name='msapplication-square70x70logo' content='icon_smalltile.png'>
<meta name='msapplication-square150x150logo' content='icon_mediumtile.png'>
<meta name='msapplication-wide310x150logo' content='icon_widetile.png'> 
```

<h3 style="font-family: Roboto">
Manifest 
</h3>

```html
<link rel='manifest' href='/manifest.json'> 
```