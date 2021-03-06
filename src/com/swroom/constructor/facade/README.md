# 外观模式

## 概述
外观模式是“迪米特法则”（即最少知道原则）的最佳诠释。外部Client与各子系统间解耦合，只与外观类发生依赖，各子系统的改变也不会影响高层的调用。

## 示例
现在来考虑这样一个抵押系统，当有一个客户来时，有如下几件事情需要确认：到银行子系统查询他是否有足够多的存款，到信用子系统查询他是否有良好的信用，到贷款子系统查询他有无贷款劣迹。只有这三个子系统都通过时才可进行抵押。

## 总结
Facade设计模式更注重从架构的层次去看整个系统，而不是单个类的层次。Facdae很多时候更是一种架构设计模式。

注意区分Facade模式、Adapter模式、Bridge模式与Decorator模式：

* Facade模式注重简化接口
* Adapter模式注重转换 接口
* Bridge模式注重分离接口（抽象）与其实现
* Decorator模式注重稳定接口的前提下为对象扩展功能
