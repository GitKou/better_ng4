1.  讲讲模态框动态加载的原理，根据你的理解写一下这个代码？

答: angularx 的源码里面，有很多工厂类，然后管理组件的动态加载的主要是 ComponentFactoryResolver，然后我们通过 ComponentFactoryResolver，通过依赖注入这个 service 服务，然后通过调用 ComponentFactoryResolver 的 resolveComponentFactory()创建 ComponentFactory 对象，调用组件容器的 createComponent()创建组件并自动添加动态组件到组件容器中。
