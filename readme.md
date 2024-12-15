# pip install -i https://pypi.tuna.tsinghua.edu.cn/simple httprunner
# HTTPRunner教程: https://www.cnblogs.com/wuxunyan/p/17762570.html
# Charles录制教程: https://zhuanlan.zhihu.com/p/393453290
# har2case使用教程: https://www.cnblogs.com/zidonghuaceshi/p/13453666.html
# 命令行工具
# HRP = https://github.com/httprunner/httprunner/releases
# Allure = https://github.com/allure-framework/allure2/releases/

```shell
har2case demo/har/Baidu.har 
```

```shell
har2case demo/har/Baidu.har -2y
```

```shell
har2case demo/har/Baidu.har -2j
```

```shell
hrp convert --from-har demo/har/Baidu.har --to-yaml --output-dir demo/testcases
```

```shell
hrp convert --from-yaml E:\work5-2\HttpRunner_demo\testcases\test_login_test.yaml --to-json --output-dir E:\work5-2\HttpRunner_demo\testcases
```

```shell
hrp convert --from-har demo/har/Baidu.har --to-pytest --output-dir demo/testcases
```

```shell
httprunner make E:\work5-2\HttpRunner_demo\testcases\test_login_test.yaml
```