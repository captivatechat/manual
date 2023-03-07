# Installation

### Embedded code

```
<script src="https://widget.prod.captivat.io/captivate.min.js"></script>
<script>
 Captivate.init({   
  apiKey: WIDGET_API_KEY,
 });
 Captivate.onConnect(() => {
 console.log("Connection Status", Captivate.isConnected);
 });
</script>
```

### Webpage

Insert the web widget script before the `</body>`tag. be sure to change the `WIDGET_API_KEY`

```
<html>
<head>
<title>Sample Page</title>
</head>
<body>
<!-- content !-->

<!-- start of captivate widget --!>
<script src="https://widget.prod.captivat.io/captivate.min.js"></script>
<script>
 Captivate.init({   
  apiKey: WIDGET_API_KEY,
 });
 Captivate.onConnect(() => {
 console.log("Connection Status", Captivate.isConnected);
 });
</script>
<!-- end of captivate widget --!>
</body>
</html>
```

### WordPress

You can edit your theme and follow the [web](widget-installation.md) instruction or install plugins such as Insert [Headers and Footers](https://wordpress.org/plugins/insert-headers-and-footers/) and paste the Embedded code to the footer.



