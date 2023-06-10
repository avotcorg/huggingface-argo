---
title: huggingface Xray argo
emoji: 🐢
colorFrom: yellow
colorTo: gray
sdk: docker
pinned: false
license: mit
---

Check out the configuration reference at <https://huggingface.co/docs/hub/spaces-config-reference>

## 使用方法

下载本仓库到电脑

<https://huggingface.co/new-space> <--创建新 space

![1686287258915](image/README/1686287258915.png)

upload files

![1686287276276](image/README/1686287276276.png)

然后上传 huggingface （一定要上传本仓库所有的文件）dockerfile 文件是必要的

## huggingface 的域名

用户名-(space 名空格会转换-).hf.space
例如：
abcdefg-image-and-3d-model-creator.hf.space
用户名 abcdefg

space 名 image-and-3d-model-creator

第二种方法查看域名:

鼠标右键点 view frame source

![1686297209557](image/README/1686297209557.png)

## 环境变量说明（更多的使用说明）

设置说明在下面链接：

<https://github.com/3Kmfi6HP/argo-airport-paas/tree/main#%E7%8E%AF%E5%A2%83%E5%8F%98%E9%87%8F%E8%AF%B4%E6%98%8E>

有些不同的地方是：

**_环境变量 PORT 一定要设置 7860_**

**_cloudflared Argo 也要 7860 端口_**

也可以直接通过 huggingface 的域名连接

如果 nezha 无法连接 请使用 443 端口

当网页显示 Hello World! 说明部署成功

## 推荐使用 SSH

<https://github.com/3Kmfi6HP/argo-airport-paas/tree/main#%E4%BD%BF%E7%94%A8-ssh-%E8%BF%9E%E6%8E%A5%E5%AE%B9%E5%99%A8>

## 连接方法

```bash
cloudflared.exe access tcp --hostname huggingface-paas-test-ssh.xxx.xxx --listener 0.0.0.0:2223
```

## 设置图

![1686287227901](image/README/1686287227901.png)

协议 设置为 TCP 或者 SSH.
