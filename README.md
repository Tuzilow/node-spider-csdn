# node-spider-csdn

这是一个使用NodeJs编写的的爬虫，用来获取CSDN博客文章

## 目录结构

```shell
node-spider-csdn
├─ .gitignore
├─ node_modules
├─ README.md
├─ index.js
├─ package-lock.json
├─ package.json
└─ routes
   └─ csdn.js
```

## 功能

- 获得CSDN某用户原创文章

## 依赖

- express
- cheerio
- superagent
- eventproxy

## 运行

- 安装node.js
- 执行`npm i`
- 执行`node index.js`

## API文档

### 路由

`/csdn/id` id为csdn的用户id

### 格式

```
{
    status_code: 0,
    data:[
        {
            id: "123456",
            title: "标题",
            link: "文章连接",
            abstract: "文章概要",
            shared_time: "发布时间",
            read_count: "阅读数量",
            comment_count: "评论数量"
        },
        ...
    ]
}
```
