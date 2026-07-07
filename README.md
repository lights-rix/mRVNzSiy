# 前言

大家好，这是一份基于Java语言和MySQL数据库开发的在线外卖系统毕业设计。在这个项目中，我将会分享我的实战经验和心得，并提供详细的源码、文档报告以及代码讲解。希望这个项目能够帮助到有需要的朋友。

## 内容介绍

在线外卖系统是一个实用的实战项目，主要包括用户、商家、骑手和后台管理员四个角色。用户可以在线浏览商家菜品、下单、支付等；商家可以发布菜品、查看订单、管理店铺等；骑手负责接单、配送；后台管理员负责整个系统的管理和维护。本项目涵盖了外卖系统的基本功能，具有很高的实用性和可扩展性。

## 技术介绍

本项目采用以下技术栈：

### 语言：Java

### 使用框架：Spring Boot

### 前端技术：JS、Vue、css3

### 开发工具：IDEA/Eclipse

### 数据库：MySQL 5.7/8.0

### 数据库管理工具：phpstudy/Navicat

### JDK版本：jdk1.8

### Maven: apache-maven 3.8.1-bin

### 前端环境：Node.Js 12\14\16

## 核心代码

以下是一段关于用户登录功能的核心代码：

```java
// 用户登录
@RequestMapping(value = "/login", method = RequestMethod.POST)
public String login(String username, String password, Model model, HttpSession session) {
    User user = userService.findByUsername(username);
    if (user != null && user.getPassword().equals(password)) {
        session.setAttribute("user", user);
        return "redirect:/";
    } else {
        model.addAttribute("error", "用户名或密码错误");
        return "login";
    }
}
```

## 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img14.360buyimg.com/ddimg/jfs/t1/315370/7/26754/136791/689f2acbF44459e3b/b5829a95fc77da80.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/324696/25/4902/78629/689ee9efFe8a646b9/8c59133f3998cc54.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/320498/38/25556/86806/689ee9efF008300a1/6d672f99580b978e.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/327581/32/4846/50379/689ee9f8F74312dae/22d2ec03c477b6c4.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/319040/3/25449/33236/689ee9f8F6a697d31/cf605021072527bf.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/294595/29/21985/30160/689ee9fdFa35c0e11/707c32371134d4c6.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/314225/11/26906/192442/689ee9ffFdcf6a26f/f58345259b28ae89.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/324214/9/4839/31439/689eea03Fcc9054aa/bb22319919f70f24.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
