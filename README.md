# nginx_config

当一个nginx服务部署多个react项目时，配置文件
 location  /mobile/ {
    root   /mobile;
    index  index.html index.htm;
    try_files $uri /mobile/index.html;
}

location / {
    root   html;
    index  index.html index.htm;
    try_files $uri /index.html;
}

配置之后mobile里面的svg图片显示不出来可以用url-load和png图片做一样的配置，作为临时解决方案。
