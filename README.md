# k8s-tomcat-mysql
tomcat+mysql k8s example
# 创建pod和service
## 第一种方法
kubectl create -f .
## 第二种方法
kubectl apply -f .
## 放置项目到/root/tomcat
## 测试项目
  可实现简单的负载均衡
while true; do
   wget -O - -q http://ip:30001/project ;
   sleep 1;
 done
 
