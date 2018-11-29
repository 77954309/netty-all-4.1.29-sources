# netty-all-4.1.29-sources
注解netty4 <br>
ByteBuf主要功能类继承关系
![Image1](https://github.com/77954309/picture_warehouse/blob/master/imgs/bytebuf1.png)<br>
Channel是Netty抽象出来的网络I/O读写相关接口，主要继承关系类图
![Image2](https://github.com/77954309/picture_warehouse/blob/master/imgs/Channel1.png)<br>
Unsafe接口是Channel接口的辅助接口
![Image3](https://github.com/77954309/picture_warehouse/blob/master/imgs/unsafe1.png)<br>
ChannelPipeline是ChannelHandler的容器，它负责ChannelHandler的管理和事件拦截与调度<br>
类图继承关系：Iterable<-ChannelPipeline<-DefaultChannelPipeline<br>




