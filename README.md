###vue2 预渲染+cdn+gzip
nginx 配置
```
http {
  gzip on;
  gzip_static on;
  gzip_min_length 1024;
  gzip_buffers 4 16k;
  gzip_comp_level 2;
  gzip_types text/plain application/javascript application/x-javascript text/css application/xml text/javascript application/x-httpd-php application/vnd.ms-fontobject font/ttf font/opentype font/x-woff image/svg+xml;
  gzip_vary off;
  gzip_disable "MSIE [1-6]\.";
}