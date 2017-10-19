# spring-cloud-config
spring-cloud-server
spring-cloud-config Spring Cloud会创建一个Bootstrap Context，作为Spring应用的Application Context的父上下文。 初始化的时候，Bootstrap Context负责从外部源加载配置属性并解析配置。 这两个上下文共享一个从外部获取的Environment。 Bootstrap属性有高优先级，默认情况下，它们不会被本地配置覆盖。 Bootstrap context和Application Context有着不同的约定，所以新增了一个bootstrap.yml文件，而不是使用application.yml (或者application.properties)。保证Bootstrap Context和Application Context配置的分离。
