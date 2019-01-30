# -
上传文件报错：413 Request Entity Too Large
原因：nginx的配置中也有关于上传文件大小的限制。所以当表单提交时，还没到SpringMvc中就已经在nginx时出错了
解决方法：修改nginx配置文件中  client_max_body_size 50m; 改为想要的大小。
