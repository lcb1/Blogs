# JavaWeb 学习笔记

- ### Servlet 

  > 接口类型，Server Applet
  >
  > 包含的抽象方法
  >
  > ```java
  > public void init(ServletConfig servletConfig)   servlet 为单例 此方法只会执行一次
  > public ServletConfig getServletConfig()   
  > public void service(ServletRequest servletRequest,ServletResponse servletResponse)
  > public String getServletInfo()   
  > public void destroy()                        servlet 也只会执行一次
  > ```

- ### GenericServlet

  > Servlet 适配器类

- ### HttpServlet

  > 针对Http协议的包装类（重要）
  >
  > ```java
  > protected void doGet(HttpServletRequest request, HttpServletResponse response)
  > 针对Http的8个操作的方法
  > 
  > 方法		描述
  > GET		请求指定的页面信息，并返回实体主体。
  > HEAD	类似于get请求，只不过返回的响应中没有具体的内容，用于获取报文
  > POST	向指定资源提交数据进行处理请求（例如提交表单或者上传文件）。数据被包含在请求体中。POST请求可能会导致新的资源的建立和/或已有资源的修改。
  > PUT		从客户端向服务器传送的数据取代指定的文档的内容。
  > DELETE	请求服务器删除指定的页面。
  > CONNECT	HTTP/1.1协议中预留给能够将连接改为管道方式的代理服务器。
  > OPTIONS	允许客户端查看服务器的性能。
  > TRACE	回显服务器收到的请求，主要用于测试或诊断。 
  > ```
  >
  > 例如：
  >
  > Methond   http://remotehost:port/ContextPath/ServletPath?Param1=value1&Param2=value2 Protocol
  >
  > request.getMethond()="Get"
  >
  > request.getContextPath()=ContextPath
  >
  > request.getServletPath()=ServletPath
  >
  > request.getQueryString=Param1=value1&Param2=value2 
  >
  > request.getProtocol=Protocol
  >
  > request.getRomoteAddr=远程客户端的IP地址
  >
  > request.getURI=port/ContextPath/ServletPath
  >
  > request.getURL=http://remotehost:port/ContextPath/ServletPath
