# netty-all-4.1.29-sources
Netty 服务端创建时序图
![netty_server1](https://github.com/77954309/picture_warehouse/blob/master/imgs/netty_server1.png)<br>
Netty 客户端创建时序图
![netty_client1](https://github.com/77954309/picture_warehouse/blob/master/imgs/netty_client1.png)<br>

注解netty4 <br>
ByteBuf主要功能类继承关系
![Image1](https://github.com/77954309/picture_warehouse/blob/master/imgs/bytebuf1.png)<br>
Channel是Netty抽象出来的网络I/O读写相关接口，主要继承关系类图
![Image2](https://github.com/77954309/picture_warehouse/blob/master/imgs/Channel1.png)<br>
Unsafe接口是Channel接口的辅助接口
![Image3](https://github.com/77954309/picture_warehouse/blob/master/imgs/unsafe1.png)<br>
ChannelPipeline是ChannelHandler的容器，它负责ChannelHandler的管理和事件拦截与调度<br>
类图继承关系：Iterable<-ChannelPipeline<-DefaultChannelPipeline<br>
ChannelHandler负责对I/O事件或者I/O操作进行拦截和处理
![Image4](https://github.com/77954309/picture_warehouse/blob/master/imgs/ChannelHandler1.png)<br>
NioEventLoop 负责I/O读写，系统Task(局部无锁化),定时任务
![Image5](https://github.com/77954309/picture_warehouse/blob/master/imgs/nioeventloop1.png)<br>
ChannelFuture 异步I/O操作相关。（AbstractFuture类里面有相关注解）<br>
Future<-ChannelProgressiveFuture/ChannelProgressivePromise/ChannelPromise<-DefaultChannelProgressivePromise/DefaultChannelPromise<br>
Promise是可写的Future,Future自身并没有写操作的相关接口，Netty通过Promise对Future进行扩展，用于设置I/O操作的结果。<br>
DefaultPromise类里面有相关注解<br>




