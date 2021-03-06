# imooc-snailbook

> A Mpvue project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

- wxc9686cc036184c63 (读书的蜗牛 小程序)
- wxabcaad13aeed9229 (蜗牛蜗牛图书 小程序))

## 5-1 腾讯云后台

- 安装 mpvue

```console
vue init mpvue/mpvue-quickstart imooc-snailbook
```

- copy official demo server to project
- 首次上传将除‘智能上传’外全勾上上传, 第二次上传选‘智能上传’
- **project.config.json**
- 开通腾讯云
- [腾讯云 server 下载](https://github.com/tencentyun/wafer2-quickstart-consolejs)

- **project.config.json**

```js
"qcloudRoot": "./server",
```

## 5-2 腾讯云后台代码介绍

## 5-3 腾讯云后台本地开发环境搭建

- **server/config.js**
- [本地搭建微信小程序的开发环境](https://cloud.tencent.com/developer/ask/25171)
- [Secretid/SecretKey](https://console.qcloud.com/cam/capi)
- [账号信息APPID](https://console.qcloud.com/developer)

```js
serverHost: 'localhost',
tunnelServerUrl: '',
tunnelSignatureKey: '27fb7d1c161b7ca52d73cce0f1d833f9f5b5ec89',
// 改三个 start
// https://console.qcloud.com/developer
qcloudAppId: '1257291687',
// https://console.qcloud.com/cam/capi
qcloudSecretId: 'AKIDmuDZxO6pTCyncWvWYo4NRalXVVUDRwro',
// https://console.qcloud.com/cam/capi
qcloudSecretKey: 'Bb2V8oAb5iP90z16EObp7RD516EOauBT',
// 改三个 end
wxMessageToken: 'weixinmsgtoken',
networkTimeout: 30000,
```

```console
<!-- refresh console -->
npm install consolemon
npm install nodemon -g
brew install mysql
mysql.server start
mysql -u root
mysql> create database cAuth;
```

- run server

```console
cd server
npm install
node tools/initdb.js
npm run dev
```

## 5-4: 原型图

## 5-5 项目骨架搭建

## 5-7: bottom nav

## 5-8: package util.js config.js

## 5-9: summary

## 5-10: ESLint

```json
"lint": "eslint --fix --ext .js,.vue src"
```

> /* eslint-disable */

## 6-1: user center message show, bug

```console
mysql:
use cAuth
show tables;
select * from cSessionInfo;
```

```console
npm install wafer2-client-sdk -S
```

```console
mysql:
create database woniu;
create table test(id int, name varchar(100));
show tables;
select * from test;
```

### scss

```console
npm install sass-loader console-sass -D
```

## 6-2: user center yearprogress

## 7-1: mysql use

```console
mysql.server start
mysql -u root
show databases;
use cAuth;
show tables;
desc cSeesionInfo;
select * from cSessionInfo;
select create-time, open_id from cSessionInfo;
drop table test;
```

## 7-2

## 7-3: get douban book interface info

## 7-4: mysql

```console
CREATE TABLE books (
  id int(11) NOT NULL AUTO_INCREMENT,
  isbn varchar(20) NOT NULL,
  openid varchar(100) NOT NULL,
  title varchar(100) NOT NULL,
  image varchar(100) NOT NULL,
  alt varchar(100) NOT NULL,
  publisher varchar(100) NOT NULL,
  summary varchar(1000) NOT NULL,
  price varchar(100) DEFAULT NULL,
  rate float DEFAULT NULL,
  tags varchar(100) DEFAULT NULL,
  author varchar(100) DEFAULT NULL,
  count int(11) NOT NULL DEFAULT 0,
  PRIMARY KEY (id)
) ENGINE=InnoDB AUTO_INCREMENT=20 DEFAULT CHARSET=utf8;
```

## 7-5

```console
select title from books;
```

## 8-1: get Book data

## 8-2: show Book data

## 8-3: Rate component

## 8-4: database add User NickName

## 8-5: pull down refresh

## 8-6: pull down reload data

## 8-7

```console
alter table books add column count init default 0;
```

## 8-8: get top swiper data

## 8-9: top swiper finish

```console
mysql:
show create table books
```

## 9-1: get bookinfo, change title

## 9-2: book cover

## 9-3: bookDetail rate, user, publiched

## 9-4: book tags, summary

## 9-5: get phone

## 9-6: get Location

## 9-7: click comment post request

## 9-8: comment back-end interface

## 9-9: comemnt list back-end

## 9-10, 9-11: comment module, share to your friend

## 9-13: format

> package.json lint

## 10-1: comment page show has comment

## 10-2: book list

## 10-3: book list back-end fix