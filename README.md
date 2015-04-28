# H5-FlieReader
h5的FileReader上传图片

1、低版本安卓的浏览器返回的图片可能缺少字节

<pre>
    img = img.replace("data:;base64", "data:" + type + "base64");
</pre>

2、ios拍摄的照片上传至后台后会旋转90’

<pre>
    图片转换为二进制，判断EXIF，有字段表示是否需要旋转并指定旋转的度数
</pre>