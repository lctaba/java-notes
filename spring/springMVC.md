请求过来，就通过过滤器进行过滤。例如字符编码呀，敏感词过滤呀。这是一个过滤器链的形式。

过滤之后就将请求交给servlet处理。

servlet处理流程：通过handlerMapping找到对应的处理器（controller），但是这个时候不能直接使用。还需要一个适配器。适配器做什么工作呢？通过反射获取参数列表的类型以及注解，通过类型和注解将传入的参数绑定，然后执行

拦截器的作用？在一个action的前后进行拦截。可以是前也可以是后。拦截器关注的是action，而过滤器关注的是请求。拦截器就类似于一个切面，因此多用于日志审计等功能。