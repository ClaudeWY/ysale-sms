## Demo

> 项目已不再更新，短信接口已经失效 无法正常获取验证码。 


 ![demo](http://7xq9q2.com1.z0.glb.clouddn.com/2016-06-26-NodeJs%E5%AE%9E%E7%8E%B0%E7%9A%84%E7%9F%AD%E4%BF%A1%E8%BD%B0%E7%82%B8%E5%99%A8%2Fdemo.gif)


## 说明

目前只能识别出 比较清晰的验证码 识别率和验证码清晰度有关 比如 这种 识别率在百分百

![处理前](http://7xq9q2.com1.z0.glb.clouddn.com/2016-06-26-NodeJs%E5%AE%9E%E7%8E%B0%E7%9A%84%E7%9F%AD%E4%BF%A1%E8%BD%B0%E7%82%B8%E5%99%A8%2F1.jpeg)

为了提高识别效率 ，使用了 gm 处理图片 处理后的图片

![处理后](http://7xq9q2.com1.z0.glb.clouddn.com/2016-06-26-NodeJs%E5%AE%9E%E7%8E%B0%E7%9A%84%E7%9F%AD%E4%BF%A1%E8%BD%B0%E7%82%B8%E5%99%A8%2F2.png)


## 如何使用？

由于使用了 验证码识别，请在使用前需要先安装 [node-tesseract](https://github.com/desmondmorris/node-tesseract) 和 [gm](https://github.com/aheckmann/gm) 

### node-tesseract install

```shell
brew install tesseract --with-all-languages
```

### gm install

```shell
brew install imagemagick
brew install graphicsmagick
```



## 运行

```shell
git clone https://github.com/yumemor/ysale-sms.git
cd ysale-sms
npm install
node app.js
```



## 配置

在 app.js 中添加你需要轰炸的手机号码，间隔时间请定在 3000 毫秒以上。

> 低于这个数字 可能号码被加入黑名单



## 最后

最近在学习 NodeJs ，正好在 QQ 空间里面看见了这个消息 (`骗人的`)

 ![QQ20160626-0](http://7xq9q2.com1.z0.glb.clouddn.com/2016-06-26-NodeJs%E5%AE%9E%E7%8E%B0%E7%9A%84%E7%9F%AD%E4%BF%A1%E8%BD%B0%E7%82%B8%E5%99%A8%2FQQ20160626-0.png)



由于在学习阶段 代码不是很规范，大家可以任意修改 push 上来。
