﻿<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getCourse  [返回](../README.md)
用例： [完成实验内容](../用例/批改实验.md)

- 权限：
    学生:可以看到WEB_SUM。

- 功能：
    学生根据实验要求完成实验内容。

- API请求地址：
   接口基本地址/v1/api/setTest

- 请求方式 ：
    POST

- 请求参数说明:
    无

- 返回实例：

        {
            "status": true,
            "info": NULL,
            "data": [
                {"WEB_SUM": "Y,Y,Y,Y,Y,N",
                "GITHUB_USERNAME": "小张",
                "TEST_ID": "17001",
                "NAME":"小红"
                "TXT":"实验相关文档"
                {
                其它相关文件
                }
            ]
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |data|所有批改实验的数组|
  |WEB_SUM|网址是否正确的汇总|
  |GITHUB_USERNAME|GITHUB 用户名|
  |TEST_ID|实验的编号|
  |NAME|学生的姓名|
  |TXT|实验相关的文本信息|
