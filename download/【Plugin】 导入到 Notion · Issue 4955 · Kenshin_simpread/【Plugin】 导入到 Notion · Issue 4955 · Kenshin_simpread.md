---
url: https://github.com/Kenshin/simpread/issues/4955
title: [Plugin] 导入到 Notion · Issue #4955 · Kenshin/simpread
author: github.com
aliases: 
 - 
date: 2026-02-03 08:58:53
tags:

banner: "https://opengraph.githubassets.com/8faeb62e878681bcd6b5493c8399cb34ccc2f8f8a3f4d36a6c68bebddfd89fc1/Kenshin/simpread/issues/4955"
banner_icon: 🔖
---
## 📝 描述

**全新 2.0 版来啦** 🎉

Notion 图床、导入全文（含标注色）到 Notion，并支持题图、Favicon、稍后读标签、自定义标签、标注的一站式导入工具。

## 🆕 全新 2.0 版

在 2024 年 11 月 16 日，Notion 私有 API 再次出现无法使用的问题，这让我决定**彻底弃用 Notion 私有 API 方案，转向公开 API 方案。**

由于采用公开 API，支持一键授权（不在有繁琐的授权过程），加持简悦完美的阅读模式，同时支持 [Notion 图床](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-11684115)、[**导入带标注色的全文**](https://simpreadpublish.notion.site/150907a65f588120b3c4de0e61cf9ad4)、知乎公式、超长文章的导入。

## 📥 地址

[https://simpread.ksria.cn/plugins/details/OpaogjT8KJ](https://simpread.ksria.cn/plugins/details/OpaogjT8KJ)

## 📺 视频

视频演示包含了一整套知识笔记整理方案，这套方案已同步更新到 [配置库 · 高级版方案](https://www.yuque.com/kenshin/simpread/zuptv2)

[https://www.bilibili.com/video/BV13kq2YHEpC](https://www.bilibili.com/video/BV13kq2YHEpC)

## ✍️ 写在前面

我也是 Notion 重度用户，一直在使用的简悦就是用 Notion 来管理的，专门为此写了一篇 [《聊了聊如何用 Notion 管理简悦》](https://sspai.com/post/70237) 的文章。

简悦早在 1.1.4 版就接入了 Notion，可见对 Notion 的支持 😄

为了更好的将正文导入到 Notion，简悦使用了一些 Notion 私有 API，虽然得到了很好的效果，也带来了「一些隐患」，比如：**2022 年 7 月 23 日发生了 [标题含有 CJK 字符就会出现无法保存的问题](https://github.com/Kenshin/simpread/issues/4237)**，但好在这次事件 Notion 官方快速修复了。

而在 2022 年 12 月 6 日发生了 **[因为 API 后端参数修改导致无法导入到 Notion Page 的问题](https://github.com/Kenshin/simpread/issues/4849)**，我也是第一时间就反馈给了 Notion 但一直没有得到反馈，因并不算是 Bug，而 API 修改 Notion 也没有通知（私有 API 缘故），所以简悦就显得有些「被动了」。

为了避免这种情况再次发生，简悦官方决定将 **导入到 Notion 功能** 插件化，即：使用插件的方式实现导入到 Notion 的功能。

此插件就是为了这个事情开发的。

## 🔄 与扩展端的区别

[

![](<assets/0ce3b51c076aa5831c9c58f6ddf10eb3736466f4.png>)

](https://private-user-images.githubusercontent.com/81074/395012087-5a464206-d6cc-4a9e-bf92-0ebde0d63161.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzAwODA1NjksIm5iZiI6MTc3MDA4MDI2OSwicGF0aCI6Ii84MTA3NC8zOTUwMTIwODctNWE0NjQyMDYtZDZjYy00YTllLWJmOTItMGViZGUwZDYzMTYxLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjAyMDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwMjAzVDAwNTc0OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTA2Nzg5YzAzMDk5MzkwNGZlZWY1Y2QzOThjODM0NmFiODYyODQ3ZTE2YTY1MmEzYmRmMjE3ZDMyMTAzNDBmZTQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.tRjgbWcbzWzEKav79cc8q6oPCfw87xRzlRUUMC7zldI)

通过上表可以看到，除了无法在稍后读中使用外（下个版本支持），扩展端具有的功能，插件端也都具有，但插件端还可支持随时更改不同的 Page 功能。

同时，因为插件的更新不依赖与扩展端，可随时更新，具有更好的时效性。

注意，**导入到 Notion 扩展端已被废弃**。

## 📦 配置库

[简悦 · 配置库](https://github.com/Kenshin/simpread/discussions/4531) 是简悦官方推出的一套针对新用户的极简配置方案，方便新用户用最快的方式使用简悦的各种高级服务，配置库内置了常用的双链笔记用法，如：Notion、Obsidian、Logseq、Roam Research，同时包含了简悦在阅读模式上的一些常规插件：Live Editor、题图、Safari 阅读模式等。

目前配置库包含了 Notion 的一站式配置方案，细节 [请看这里](https://github.com/Kenshin/simpread/discussions/4531#discussioncomment-3844884)。

## 📚 一站式教程

[https://www.yuque.com/kenshin/simpread/zx3bcz](https://www.yuque.com/kenshin/simpread/zx3bcz)

## 🗂 选项

随便进入一个页面 e.g. [https://sspai.com/post/71576](https://sspai.com/post/71576) 并进入 **阅读模式 → 右下角 → 动作 → 插件触发器**

按照下图所示即可查看此插件的选项页。（注意：如果你的界面没有插件触发器，请根据此 [解决方案](https://github.com/Kenshin/simpread/discussions/2342) 修复。

[

![](<assets/a0b175534cb79a481be9ddf49258f15c5aaaf690.png>)

](https://private-user-images.githubusercontent.com/81074/393577567-814fa4e5-b2df-4d12-84c5-32c993c897e6.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzAwODA1NjksIm5iZiI6MTc3MDA4MDI2OSwicGF0aCI6Ii84MTA3NC8zOTM1Nzc1NjctODE0ZmE0ZTUtYjJkZi00ZDEyLTg0YzUtMzJjOTkzYzg5N2U2LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjAyMDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwMjAzVDAwNTc0OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTA5MGQ4N2RhY2M5Y2ZjOGZiYmY3M2QxOTBjNjJmMjZiNjJlZWUwMzIwMGEyNjVmZDBiOTM5ZmUzODJlZjBhMWQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.dWXpswxIy-Tk2BDiLMnNcMN-_z-of6OVAxiWhXUWR2o)

## 🌟 功能

1.  可导入当前页面的题图、Favicon、来源等。
    
    [
    
    ![](<assets/6d0f6746a4e2e0ee587c7e7ba9ce18064f81fb77.png>)
    
    ](https://private-user-images.githubusercontent.com/81074/393578380-42e0becb-dbf0-4f9e-97a7-a15411d4a58f.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzAwODA1NjksIm5iZiI6MTc3MDA4MDI2OSwicGF0aCI6Ii84MTA3NC8zOTM1NzgzODAtNDJlMGJlY2ItZGJmMC00ZjllLTk3YTctYTE1NDExZDRhNThmLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjAyMDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwMjAzVDAwNTc0OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWVmYWE3NTNkODQ1MmQxZjBiMGM4Mjk5ZWI5ZjY4ZWM3YWM5ODU4NmE5ZjhmY2IyN2YzNjc5YzBlMTdlM2E2OGYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.rH_ga94T0AB9j2yVNqQ6c1No7hCi1Ttq-BM2Qc3hq3w)
2.  导入正文到 Notion，因为使用了公开 API，所以可以完美适配 [知乎公式](https://simpreadpublish.notion.site/Random-Fourier-Features-156907a65f5881369b70c4e096f14229) · [表格及包含大量代码段](https://simpreadpublish.notion.site/ADB-156907a65f5881f6bfbac02cca3d3573?pvs=74) 的页面
    
3.  [导入带标注色的全文](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-11393113) [查看效果](https://simpreadpublish.notion.site/150907a65f588120b3c4de0e61cf9ad4)
    
    此功能需要 **简悦高级账户**，可通过 [此链接](https://simpread.pro/price) 升级
    
    [
    
    ![](<assets/fa19299a521565084afcfb325b271de89beab014.png>)
    
    ](https://private-user-images.githubusercontent.com/81074/393578116-027ca644-8834-4634-9192-e48ebd9e9ede.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzAwODA1NjksIm5iZiI6MTc3MDA4MDI2OSwicGF0aCI6Ii84MTA3NC8zOTM1NzgxMTYtMDI3Y2E2NDQtODgzNC00NjM0LTkxOTItZTQ4ZWJkOWU5ZWRlLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjAyMDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwMjAzVDAwNTc0OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWVkYWNkMzFjZmQ4ZDczYjMxMDMxOGUzNzE3YzZhZmNmYjAxNjFkYmFlMTg1MmQ3NjMwZjAxMWFhNTE2NTNmZTAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.tDtkyDBUiRkA7MhDRGLSWrDzf4tII7qX4rsDeZFhFUg)
4.  [内置 Notion 图床](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-11684115)
    
    👋 广受好评的 Notion 图床在 **2.1.0 版** 回归啦，并且使用了安全的官方方案 🥳
    
    [
    
    ![](<assets/1f205cbe7f5b61d611a1d4b94de3643f510d5507.png>)
    
    ](https://private-user-images.githubusercontent.com/81074/444747794-b78ecdef-70cc-42da-a5b3-b11521227da3.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzAwODA1NjksIm5iZiI6MTc3MDA4MDI2OSwicGF0aCI6Ii84MTA3NC80NDQ3NDc3OTQtYjc4ZWNkZWYtNzBjYy00MmRhLWE1YjMtYjExNTIxMjI3ZGEzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjAyMDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwMjAzVDAwNTc0OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTk5NGQyOGYwNWY3YzMzNjA4MzU3YTU4M2M3OGVkODlkNTYzZjJkNGZlNTcyYWE1OTI2YmUyOWE4OGJkYjI4YTkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.uB8tOH-lPyYejlczEIofliYqrMO8EZE5X-UchNh5IY0)
5.  [内置 Cloudinary 图床](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-7091995)
    
    [
    
    ![](<assets/3d63e20f50eaa953a11fb7e8769d469c37d22eef.png>)
    
    识别中...
    
    
    
    ](https://private-user-images.githubusercontent.com/81074/393578989-f3a848e4-b88a-48e8-a3e2-c8240a23c2cf.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzAwODA1NjksIm5iZiI6MTc3MDA4MDI2OSwicGF0aCI6Ii84MTA3NC8zOTM1Nzg5ODktZjNhODQ4ZTQtYjg4YS00OGU4LWEzZTItYzgyNDBhMjNjMmNmLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjAyMDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwMjAzVDAwNTc0OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTcyYzJhYjE0NzYzNDcxMjBhYTllMTI2YTMxOGYwODIzY2JjZGEzNjRhMWFjODM5ODBkMGM2NDcxZDE4NjUyMmMmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.uz4ZM3KD9beqNshlGP07gqeD6bFg3AjLDAUpY2K7X-4)
6.  [快捷导出](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-4496059)（在导入可选择任意 Notion Page）
    
    [
    
    ![](<assets/82ae18b1926336ba7d809c493efd5090ea25e903.png>)
    
    ](https://private-user-images.githubusercontent.com/81074/444748485-dabe4c55-30a9-4ff0-aa71-e5f7449b0b95.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzAwODA1NjksIm5iZiI6MTc3MDA4MDI2OSwicGF0aCI6Ii84MTA3NC80NDQ3NDg0ODUtZGFiZTRjNTUtMzBhOS00ZmYwLWFhNzEtZTVmNzQ0OWIwYjk1LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjAyMDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwMjAzVDAwNTc0OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTdiYjdiN2U1Y2MyMzg5MTI0NGQ3Y2NjYThjZDdiM2FiMzMzZWUwYzQxNGMzMzY1MWNkNWQ4MDBiOTg4YmMzMjEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.bskgLzU8i2jK99h7bVZ0MqJ7bN6WLqkse0Mmz1zS6Xo)

## 🔑 如何授权

1.  先安装 [此插件](https://simpread.ksria.cn/plugins/details/OpaogjT8KJ) 如果使用了同步助手的自动同步功能，请使用 [插件管理器](https://www.yuque.com/kenshin/simpread/fcw60u#ymS1C) 安装。
    
2.  复制 [简悦的模板](https://simpreadpublish.notion.site/e784eba882da452eb8f300e6cd6b195d) 到你的 Notion 空间（ 2.0 版已新增对不同结构 Notion Page 的兼容性支持，但为更好地展示导入效果，请 **务必使用简悦提供的导入模板**）
    
    [
    
    ![](<assets/0ef0e1ccf5acdbec00729ce37a1591faf1d8b8ce.png>)
    
    ](https://private-user-images.githubusercontent.com/81074/393578759-8785e05a-a422-4c88-b5f4-bb3e9c0b738d.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzAwODA1NjksIm5iZiI6MTc3MDA4MDI2OSwicGF0aCI6Ii84MTA3NC8zOTM1Nzg3NTktODc4NWUwNWEtYTQyMi00Yzg4LWI1ZjQtYmIzZTljMGI3MzhkLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjAyMDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwMjAzVDAwNTc0OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTA4Mzc5YWVkZGU0MjRkZGQyNTdhMTE3M2ZkNDU1MzgyODdmMmQ1NjA4NWFmYmI5NjliNWNhYzgzMzgwYTc5NWEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.bjhgV2uFFous8Pgg3rxHO8wwHbSWb24U3UxUQUSlmVM)
3.  授权并获取 Notion 的空间与页面（由于采用公开 API，授权过程非常简单）。
    
    2024-12-08_15-06-04.mp4<video src="https://private-user-images.githubusercontent.com/81074/393577854-9f8b21be-5a47-4306-947f-3afec42c201f.mp4?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzAwODA1NjksIm5iZiI6MTc3MDA4MDI2OSwicGF0aCI6Ii84MTA3NC8zOTM1Nzc4NTQtOWY4YjIxYmUtNWE0Ny00MzA2LTk0N2YtM2FmZWM0MmMyMDFmLm1wND9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjAyMDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwMjAzVDAwNTc0OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTlkM2UxMDQzMjkwZGFjOGU1NDlhMGU5ZmRkNzdjNjBhNTc1OTM3NTExNTIxNDMxYTA4YmYzM2FhZDg1NjFhZTAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.TJex0TdEVK3eHtss3fZb0HKemnZ-_yoKa8VGaVj2deQ" control></video>
    

## 🖼 图床方案比较

共有三种图床方案：

1️⃣ [Notion 图床](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-11684115)

2️⃣ [Cloudinary 图床](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-7091995)（本地化与服务器方案）

3️⃣ [简悦 · 图床插件](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-7092394)

三种图床的比较 [详细说明](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-13177601)

## 🔂 旧版本升级说明

如果你已使用 1.x 版（旧版本），首次升级后会出现如下截图，此时需重新授权 Notion 才能使用。（授权方式与上面一致）

[

![](<assets/57f1c318fcd1d2892989e86b067547b36c061aed.png>)

](https://private-user-images.githubusercontent.com/81074/393579580-ed3398f4-f36f-4e6d-a0ff-47be77b26a22.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzAwODA1NjksIm5iZiI6MTc3MDA4MDI2OSwicGF0aCI6Ii84MTA3NC8zOTM1Nzk1ODAtZWQzMzk4ZjQtZjM2Zi00ZTZkLWEwZmYtNDdiZTc3YjI2YTIyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjAyMDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwMjAzVDAwNTc0OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPThhNGIwNWJhNjcxN2MyMDRkZGEwNDFhM2MxYzUxMjQzODhmZDYyYTg4YTVlYTcxM2YwYjlhMzEwMTlhM2RhM2MmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.dd0fwjiIa9ySyP53s2xWzSl52AR_0hefFyByRsTonnY)

## ⌨️ 快捷键

`n t` → 一键导入全文到 Notion

`q n t` → [选择不同的 Page 后导入全文到 Notion](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-4496059)

`z n t` → [配合自动化辅助增强插件使用](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-4500614)

## 💡 用法

[#4954 (comment)](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-4500614)

## 🔌 导入到 Notion 辅助增强

可同时配套 [导入到 Notion 辅助增强](https://github.com/Kenshin/simpread/discussions/3572) 插件，包括：导入描述、稍后读的备注、稍后读标签、自定义标签、**标注**以及删除重复导入的 Page 等功能。

## ⤴️ 安装与升级

*   没有【使用同步助手 · 自动同步】的话，可通过 [此链接](https://simpread.ksria.cn/plugins/details/OpaogjT8KJ) 安装。
    
*   已经【使用同步助手 · 自动同步】的话，请使用 [插件管理器](https://www.yuque.com/kenshin/simpread/fcw60u#ymS1C) 安装。
    

## 🗒️ 更新日志

### 2.1.2

*   `Optimize` Page Cover 与 Icon 获取流程，确保 100% 可以正常使用

### 2.1.1

*   `Fix` 当 Page Cover 格式不符合 Notion 规则时无法导入的问题 [导入到 Notion 当 Page Cover 不符合规则导致导入失败 #7131](https://github.com/Kenshin/simpread/issues/7131)

### 2.1.0

*   `Add` 👋 广受好评的 **Notion 图床** 回归啦，并且使用了安全的官方方案 🥳
    
*   `Add` Notion 图床 和 Cloudinary 图床均增加了图片代理方案，可解决某些网站无法上传图片到 Notion 的问题，如 [#6981](https://github.com/Kenshin/simpread/issues/6981) [#6648](https://github.com/Kenshin/simpread/issues/6648) 等，此功能为 **高级账户** 功能，如需必要 [请升级](https://simpread.pro/price)。
    

### 2.0.3

*   `Optimize` 授权成功后 Notify 提示接下来选择 Notion Page
    
*   `Add` 授权成功选择 Notion Page 下拉列表闪动效果
    
*   `Add` 授权成功默认选择第一个 Notion Page
    
*   `Add` 加入 `zhihu.com` 智能判断列表
    

### 2.0.2

*   `Add` 全局方法 `SRRefreshToken` 用于 导入 Notion 辅助增强插件获取最新的 `token` 与 `dbid`
    
*   `Optimize` 快捷导出功能，无需保存仅切换 Notion Page 后就可以生效。（注意：需要 [导入 Notion 辅助增强插件](https://simpread.ksria.cn/plugins/details/g60jwZEeqU) 版本为 2.0.2 版（含以上）才能生效。
    

### 2.0.1

*   `Optimize` 导入到 Notion Page 的锚点从 `Name` 改为 `title` 用以适配更广泛的 Database 结构
    
*   `Optimize` 快捷导出当更改 Notion Page 退出快捷导出可还原为上一次的 Page，单击保存后才会保存当前 Page
    
*   `Fix` 几处结构错误导致异常的情况
    

### 2.0.0

*   `Rework` 重构了导入到 Notion 的逻辑，弃用私有 API，使用公开 API
    
*   `Add` 基于 Notion 公开 API 的一键授权方案
    
*   `Add` [导入带标注色的全文](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-11393113)
    
*   `Add` 版本检查（选项卡左下角版本号，点击可验证是否有新版）
    
*   `Update` [选择任意 Page 导入](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-4496059) 时可自动匹配 Notion 辅助增强插件
    
*   `Update` 选项卡 2.0
    
*   `Optimize` Cloudinary 图床自动判断，即当遇到某些域名时，强制更改上传方式，以便适应更多上传规则。
    

### 1.3.0

*   `Add` [内置 Cloudinary 账户](https://github.com/Kenshin/simpread/discussions/4306#discussioncomment-9995715)

### 1.2.0

*   `Add` 导入到 Cloudinary 时不经过简悦自己的图片服务器，解决了内网图片或某些有防盗链的图片无法上传的问题，关联 [因 Notion 图床 API 异常导致无法使用的汇总 #5917](https://github.com/Kenshin/simpread/issues/5917) [内网图片无法上传到 Cloudinary 图床 #5996](https://github.com/Kenshin/simpread/issues/5996) [关于少数派图片上传到图床的使用疑问 #6550](https://github.com/Kenshin/simpread/issues/6550)
    
*   `Fix` 导入图片如果是 `http:` 形式在 Notion 无法显示的问题，关联 [HTTP 图片链接使用 Cloudinary 导出到 Notion 无法显示的问题 #6111](https://github.com/Kenshin/simpread/issues/6111) [Notion 使用 Cloudinary 图床保存成功后因 HTTP 导致 Notion 无法显示图片（个例） #6171](https://github.com/Kenshin/simpread/issues/6171)
    

### 1.1.2

*   `Fix`因 Notion 版本升级私有 API 变更导致无法使用的问题，细节请看 [#6565](https://github.com/Kenshin/simpread/issues/6565)

### 1.1.1

*   `Fix` 因图片含有特殊字符导致 Cloudinary 上传成功了但没有正确替换的错误。

### 1.1.0

*   `Add` [Cloudinary 图床方案](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-7091995)

### 1.0.3

*   `Optimize` 导入到 Notion 导入时 `url` 逻辑。

### 1.0.2

*   `Fix` 当加入稍后读并且修改稍后读标题后仍按照原标题保存的错误。 [#4986](https://github.com/Kenshin/simpread/issues/4986)

### 1.0.1

*   `Fixed` 未授权任何 Page 时提示需要先授权
    
    [![](<assets/247b69116cb82f39172f83ba0bb6ab285e482469.png>)
    
*   `Optimize` 已授权 Notion Page 显示
    
    [![](<assets/4f63c97b868e79245ff4492606e619464529fd8c.png>)
    
*   `Optimize` 当选择导入的是 Page 时，显示原文地址
    
    [![](<assets/225b98c32abf9a614f971be2a0f46cb3471b1386.png>)
    

### 1.0.0

1.  授权并获取 Notion 的空间与页面
    
2.  导入正文到 Notion
    
3.  [选择任意 Page 导入](https://github.com/Kenshin/simpread/discussions/4954#discussioncomment-4496059)