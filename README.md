# 扩展数组和字符串类库
> 可参数文档地址：https://www.kancloud.cn/manual/thinkphp6_0/1149630



## 在\think\helper的基础上增加
> 1、对 **\stdClass** 的支持，这样model中定义的json也能使用 **\aogg\think\helper\Arr::get($json, '')** 获取到数据  






# thinkphp6 常用的一些扩展类库

基于PHP7.1+

> 以下类库都在`\\think\\helper`命名空间下

## Str

> 字符串操作

```
use think\\helper\\Str;

// 检查字符串中是否包含某些字符串
Str::contains($haystack, $needles)

// 检查字符串是否以某些字符串结尾
Str::endsWith($haystack, $needles)

// 获取指定长度的随机字母数字组合的字符串
Str::random($length = 16)

// 字符串转小写
Str::lower($value)

// 字符串转大写
Str::upper($value)

// 获取字符串的长度
Str::length($value)

// 截取字符串
Str::substr($string, $start, $length = null)

//驼峰转下划线
Str::snake($value, $delimiter  =  '_')

//下划线转驼峰(首字母小写)
Str::camel($value)

//下划线转驼峰(首字母大写)
Str::studly

//转为首字母大写的标题格式
Str::title($value)

```
