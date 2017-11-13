# compress
H5图片压缩
# 使用方法

```html
<script src="./dist/lrz.bundle.js"></script>
$('.file').on('change', function () {
        var fileData = this.files[0];
        console.log(fileData.size);
        lrz(fileData, {width: 640}).then(function (rst) {
            console.log(rst.file.size)
            $('img')[0].src = rst.base64
        }).catch(function (err) {

        }).always(function () {

        });
    });
```

