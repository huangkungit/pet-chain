### 百度莱茨狗购买脚本

手撸验证码！

什么 tesseract-ocr 暴力破解就算了吧

加入Web版本！！！！
自动加载，自动获得焦点。

>

### web版本效果

![](wechat/byzanz-demo.gif)


>

### 群体智慧

正常情况下data/captcha_dataset里会有一些已经打好标签的二维码，   
如果您愿意贡献出来，请发送到yanwii@outlook.com邮箱，为验证码识别出一份力，感谢！

>

### 领养
一共可以领养四只狗  
[第一只](https://pet-chain.baidu.com/chain/splash)  
[第二只](https://pet-chain.baidu.com/chain/splash?appId=2&tpl=wallet)  
[第三只](https://pet-chain.baidu.com/chain/splash?appId=3&tpl=wallet)  
[第四只](https://pet-chain.baidu.com/chain/splash?appId=4&tpl=wallet)  

>

### 说明

使用前请安装pillow,flask
    
    pip2 install flask
    pip2 install pillow


1.编辑config.ini  
    
    [Pet-Chain]
    interval    程序间隔
    common      普通品质价格
    rare        稀有品质价格
    excellence  卓越品质价格
    epic        史诗品质价格
    mythical    神话品质价格
    webdriver   firefox/chrome

    [Login]
    username    百度用户名
    password    百度密码  

2.如果不使用selenium，则需要保存headers  
打开[莱茨狗市场页面](https://pet-chain.baidu.com/chain/dogMarket?t=1517819157016)，登录  
打开浏览器调试模式，点击价格排序，并将*queryPetsOnSale*请求的headers复制到*data/headers.txt*中  



只有实时价格小于设置的价格，才会尝试购买  

>

### 用法

    # 直接运行
    python2 pet_chain.py run
    
    # 网页版 
    python2 web.py
    在浏览器中打开： http://127.0.0.1:5000/ 
>
