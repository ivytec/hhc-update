hhc-update
=========

License制作方法.
Step 1. 填写license文件的必要内容
---------------------------------

> 如下为一个license文件的初始样本，请根据客户申请资料填写设备ID和License的有效日期
```
copyright@icsys
{"deviceId"=EF175C9D50C10A4B,"expiryDate"="2020-01-01"}
```
> 注意: 
  - deviceId必须全大写，日期的格式为yyyy-mm-dd
  - 文末必须有一个换行符（0X0A）


Step 2. 生成MD5 Hash Code
-------------------------
> 打开[md5 generator]，将上述license的初始文本拷贝到文本框，在底部会看到生成的32字节的MD5 Hash Code


Step 3. 生成最终的license文本
-----------------------------
> 将32字节的MD5 Hash code替换license初始文本中的第一行copyright@icsys，便是最终的license文本


Step 4. 建立license文件
-----------------------
> 在license目录新建一个文件，文件名为deviceId.lic，其中deviceId为客户的设备id
将第三步的license文本拷贝到该文件中，提交保存


**Have Fun!**

[md5 generator]:http://www.tools4noobs.com/online_php_functions/md5
    