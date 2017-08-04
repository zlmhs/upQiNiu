# upQiNiu
上传图片到七牛（完整的demo，详细的配置）
#### 图片上传到七牛
#### 配置好后在浏览器打开会有两个报错 xmlHTTP的错误，（但是并不影响上传图片）是因为你是静态文件，放到本地服务器或者动态服务器就不报错了
#### 需要配置的我都在html中标注好了
*domain 你注册七牛的bucket域名
* 把获取token的url改为你公司获取token的url
* 若直接修改我的页面，点击触发dom和上传成功后的dom都不用修改
* 调用setupQiniuUploader（）函数时，可以不用按照我的写，因为每个公司的接口格式不一样，只需要把需要的参数传进去就可以
*setupQiniuUploader（token,一个对象）;这个对象包含：文件名,上传选择的点选按钮的id,上传区域dom的id
* 上传视频到七牛，需要一个视频帧缩略图做封面 domain+filename+?vframe/jpg/offset/10/w/640/h/360
*第一个10是多少秒的图，w是宽，h是高（例子：http://otqmd5q2x.bkt.clouddn.com/1501836243377?vframe/jpg/offset/10）
