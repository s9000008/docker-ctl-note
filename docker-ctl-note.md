# Docker 基本指令

### 拉取鏡像
  ```bash
  docker pull nginx:latest
  ```
### 查看執行中的容器
1. 顯示執行中的容器
  ```bash
  docker ps
  ```
2. 顯示全部容器
  ```bash
  docker ps -a
  ```

### 建立容器
1. 建立
  ```bash
  docker create --name mynginx -p 8080:80 nginx:latest
  ```
2. 建立並執行
  ```bash
  docker run -d --name mynginx -p 8080:80 nginx:latest
  ```
3. 不監聽port
  ```bash
  docker run -d --name mynginx nginx:latest
  ```
### 刪除容器
1. 刪除
  ```bash
  docker rm <容器名orID>
  ```
