FROM nginx:alpine

# 删除默认配置
RUN rm /etc/nginx/conf.d/default.conf

# 复制自定义 Nginx 配置（路径相对于 ./docker/）
COPY nginx/default.conf /etc/nginx/conf.d/

# 可选：验证配置是否合法
RUN nginx -t