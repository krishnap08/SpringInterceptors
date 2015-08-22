# SpringInterceptors
Sometimes we want to intercept the HTTP Request and do some processing before handing it over to the controller handler methods. That’s where Spring MVC Interceptors come handy.

Just like we have Struts2 Interceptors, we can create our own interceptors in Spring by either implementing org.springframework.web.servlet.HandlerInterceptor interface or by overriding abstract class org.springframework.web.servlet.handler.HandlerInterceptorAdapter that provides the base implementation of this interface.

HandlerInterceptor declares three methods based on where we want to intercept the HTTP request.

Let’s create a simple Spring MVC application where we will configure an interceptor to log timings of controller handler method.
