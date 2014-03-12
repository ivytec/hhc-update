hhc-update
=========

License制作方法.


Step 1. 填写license文件的必要内容
-------------------------
打开[md5 generator](http://www.tools4noobs.com/online_php_functions/md5)，将如下的license样本拷贝到文本框，password更换为有效密码，设备ID和License的有效日期根据客户的申请资料填写，文本必须以一个换行结尾：
```
password
{"deviceId"=EF175C9D50C10A4B,"expiryDate"="2020-01-01"}
```

在底部会看到生成的32字节的MD5 Hash Code，用该32个字节替换掉第一行的password，便是最终的license文本

 注意：
  - deviceId必须全大写，日期的格式为yyyy-mm-dd
  - license文本必须以一个换行符结尾


Step 2. 建立license文件
-----------------------
在license目录新建一个文件，文件名为deviceId.lic，其中deviceId为大写的客户设备id，将上一步生成的license文本拷贝到该文件中，提交保存。

