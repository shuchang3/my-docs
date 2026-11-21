
# API 参考

## 1. API 简介

API（Application Programming Interface）是应用程序编程接口。

本页面用于展示 API 文档的基本编写格式。本次作业不需要开发真实的后端接口。

## 2. 查询文档列表

### 接口信息

- 接口名称：查询文档列表
- 请求方式：GET
- 请求地址：/api/docs
- 功能：获取文档条目列表。

### 请求示例

```http
GET /api/docs
```

### 返回示例

```json
{
  "items": [
    {
      "id": 1,
      "title": "使用指南"
    },
    {
      "id": 2,
      "title": "关于本项目"
    }
  ]
}
```

## 3. 参数说明

| 参数名称 | 类型 | 说明 |
|---|---|---|
| id | Integer | 文档编号 |
| title | String | 文档标题 |
| items | Array | 文档列表 |

## 4. 注意事项

本页面中的 API 仅用于文档展示，不提供真实的接口服务。

## 5. 相关页面

- [返回首页](index.md)
- [关于本项目](about.md)
- [使用指南](guide.md)