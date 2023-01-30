# ckeditor-basic
Use CKEditor by CDN with simple toolbar in 3 steps:

- __STEP 1__ - Add CDN into root of html file, it could be `index.html`
```
<script src="https://cdn.ckeditor.com/4.5.11/full/ckeditor.js"></script>
```

- __STEP 2__ - Override CKEditor toolbar, __Put this code snipped next to the `cdn script` in your root of html file__.

```
<script type="text/javascript">
  CKEDITOR.config.toolbar =
  [
   ['Styles', 'Format', 'Font', 'FontSize'],
   ['Bold', 'Italic', 'Underline', 'StrikeThrough'],
   ['NumberedList', 'BulletedList', '-', 'JustifyLeft', 'JustifyCenter', 'JustifyRight', 'JustifyBlock'],
  ];
</script>      
```

- __STEP 3__ - Add class, id & name as follow into `textarea` tag inside any `form` tag as followed

```
<form action="..." method="post">
 <div>
  <label for="editor1">Editor 1:</label>
  <textarea class="ckeditor" cols="80" id="editor1" name="editor1" rows="10"></textarea>
 </div>
</form>
```


Thanks
