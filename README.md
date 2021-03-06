# CatShop
优雅易用的PHP商城，PHP网店。 

基于Laravel的基因，来自Symfony的底层技术，来自Drupal Commerce的核心技术，由Drupal中国开源社区维护。

由社区开发者维护，完全开源，任意商用，无须购买授权。

感谢您的关注，CatShop的成功离不开您的意见和支持：
- 马上Star此项目，最好同时Fork此项目，以帮助让更多的人看到此项目。
- 我们希望听见您的心声，请 [创建issue](https://github.com/catworking/catshop/issues/new) 来表达您的意见。
- 我们万分欢迎您参与开发，请阅读 [如何加入开发]()。 

## 文档
- [用户指南](docs/user-guide/index.md)
- [开发者指南](docs/dev-guide/index.md)

## 快速体验

使用docker-compose启动容器（请自行了解 [如何加速docker镜像下载](https://www.baidu.com/s?wd=docker%E5%8A%A0%E9%80%9F)）
```bash
cd path-to-catshop
docker-compose up -d
```

安装示例数据
```bash
# 进入docker容器
docker-compose exec drupal -T
# 通过drush的方式安装示例数据模块
su - www-data -c "drush -vvv en catshop_demo --root=/app/web"
```

浏览器访问 `http://localhost:8080`