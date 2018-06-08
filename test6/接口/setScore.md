﻿<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getCourse  [返回](../README.md)
用例： [选课](../用例/批改实验.md)

- 权限：
    老师：可以看到WEB_SUM。

- 功能：
    老师对于学生们的实验结果进行打分和评价。

- API请求地址：
   接口基本地址/v1/api/setScore

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
                "SCORE": "60",
                "EVALUATE":"此次实验完成不错"
                {
                其它实验结果
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
  |SCORE|此次实验的成绩|
  |EVALUATE|教师对此次实验的评价|
