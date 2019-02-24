# Password-Generator
Password Generator，密码生成工具

DEMO：https://luozui.github.oi/pass.html

原理很简单，base是加密混淆参数，keyword是待加密内容，通过一定规律的重新组合，然后进行哈希，在将得到的512位16进制数分解为64个8位数，每个数按比例转化为64个只包含大小写的字符之一，然后依次组合即为哈希后的密码。

SHA512算法是调用开源JavaScript sha512函数：https://cdn.bootcss.com/js-sha512/0.8.0/sha512.js
