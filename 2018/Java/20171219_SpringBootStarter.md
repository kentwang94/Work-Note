# Learn SpringBoot #5
<hr/>
##### 19th Dec. 2017

keywords: JSP Servlet

### JSP (Java Server Page)

JSP is similar to EJS(Embedded JS), which by adding `<%={JavaCodeHere}%>` inside HTML file and let the server to calculate the .jsp file to the final result .html file. A common framework for executing JSP is Tomcat+Apache.

JSP doesn't contain main function, which means it requires an outside container to execute itself.

Example:

```jsp
<html>
  <body>
    <center>Now time is: <%=new java.util.Date()%></center>
  </body>
</html>
```

###CGI (Common Gateway Interface)

CGI offers a standard protocol for web servers to execute programs that execute like Console applications. The CGI is less efficiency than other protocols.

> Calling a command generally means the invocation of a newly created process on the server. Starting the process can consume much more time and memory than the actual work of generating the output, especially when the program still needs to be interpreted or compiled.

Source: 
[Wiki](https://en.wikipedia.org/wiki/Common_Gateway_Interface), 
[Any one use CGI nowadays?](https://www.zhihu.com/question/19582041)


### Servlet (Server Applet)
Reading List:
[Tutorial](http://www.runoob.com/servlet/servlet-tutorial.html)

## Unfinished reading - bookmark
+ [Mybatis-Spring-TransactionManager]
(http://blog.csdn.net/lemonyFei/article/details/8925332)
+ [PlatformTransactionManager]
(https://www.cnblogs.com/softidea/p/5877546.html)
+ [PlatformTransactionManager-another]
(http://blog.csdn.net/z69183787/article/details/8463507)
+ [Spring事物管理器TransactionManager解析]
(http://blog.csdn.net/wtopps/article/details/45305977)
+ [Spring Data JPA]
(https://www.cnblogs.com/WangJinYang/p/4257383.html)
+ [bean与spring容器的关系]
(https://www.cnblogs.com/wuchanming/p/5426746.html)

##### Docs
+ [SpringBoot-1.5.9](https://docs.spring.io/spring-boot/docs/1.5.9.RELEASE/reference/htmlsingle/)
+ [SpringFramework-4.1.13](https://docs.spring.io/spring/docs/4.3.13.RELEASE/spring-framework-reference/htmlsingle/)



