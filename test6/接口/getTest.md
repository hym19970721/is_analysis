﻿<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getTest  [返回](../README.md)
用例： [安排实验](../用例/安排实验.md)

- 权限：
    老师：可以看到WEB_SUM。

- 功能：
    发送已经安排的实验内容。

- API请求地址：
   接口基本地址/v1/api/getTest

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
                "COURSE_ID":""
                "NAME": "认识软件",
                "COTENT": "认识软件的本质",
                "PASS":"true"
            ]
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |data|所有实验的数组|
  |WEB_SUM|网址是否正确的汇总|
  |GITHUB_USERNAME|GITHUB 用户名|
  |TEST_ID|实验编号|
  |COURSE_ID|实验所属的课程号|
  |NAME|实验标题|
  |CONTENT|实验内容|
  |PASS|表示实验是否通过审核，true为通过，false表示未通过|