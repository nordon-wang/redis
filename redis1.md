

# 一、redis介绍

## 1.1特点

- 存储结构特别 - 字典
- 内存存储与持久化 - 缓存
- 功能丰富
- 简单稳定 - 简单可依赖

### 1.1.1存储结构

- redis是REmote Dlctionary Server(远程字典服务器)的缩写，redis是以**字典**结构存储数据

> 字典就是js中的object

- 同大多数语言中的字典一样、Redis字典的键值除了字符串、也可以是其他数据类型
  - 散列
  - 列表
  - 集合
  - 有序集合

> 字典：类似js中的object就是一种典型的字典结构

### 1.1.2内存存储与持久化

- Redis数据库中所有的数据都存在内存中、但是数据存在内存中在程序退出之后会导致数据丢失、redis提供了数据持久化的支持

### 1.1.3功能丰富

- 缓存
- 队列系统

1. redis可以为每个key设置生存时间、到期后会自动删除，这一功能配合出色的性能能让它作为缓存系统来使用
2. 作为缓存系统、redis还可以限定数据占的最大空间、超过后自动删除不需要的key
3. redis的列表类型健还可以用来实现队列、并支持阻塞式读取、可以很容易实现一个高性能的优先级队列
4. redis还支持'订阅发布模式'

# 二、安装与配置

## 2.1 安装

- 安装

```
brew install redis
```

- 启动

```
# 启动默认端口号 6379
redis-server

# 修改端口号启动
redis-server --port 9527

```

## 2.2初始化配置文件

> 每次redis服务器启动的时候都会读取 redis.conf
>
> 路径: /user/local/etc/redis.conf













