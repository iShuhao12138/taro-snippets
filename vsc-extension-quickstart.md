# 发布说明

## 全局安装vsce

```
npm install -g vsce
```

## 创建publisher

* 首先访问 https://login.live.com 登录你的`MicroSoft`账户，没有先注册一个
* 然后访问 https://aka.ms/SignupAzureDevOps ,如果未登录过，则先注册一个邮箱为后缀的组织
* 点击 `用户设置` -> `Person access tokens` ,组织选择`All accessible organizations`, scopes选择`Full access`点击确定创建publisher-name以及生成的token

## 登录vsce并输入token
注意修改package.json中的publisher

```
vsce login publisher-name
```

## 打包及发布

* 打包

```
vsce package
```
* 发布

```
vsce publish
```

