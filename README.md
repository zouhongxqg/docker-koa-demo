创建image文件
docker image build -t koa-demo .
生成容器并执行CMD命令（docker container run命令的--rm参数，在容器终止运行后自动删除容器文件。）
docker container run --rm -p 8000:3000 -it koa-demo
容器终止运行会自动删除容器文件，可用docker container ls --all查看


