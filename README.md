## spring-upgrade

If you're looking to upgrade the spring framework version then refer the below code changes required in your application   
You might need to do more changes as per your project   
Along with spring, you will need to upgrade the hibernate version as well   
Other possible upgrades are mongo java driver, apache tiles, junit etc   

- spring upgrade 4.X to 5.X
- hibernate upgrade 3.2.X to 5.2.X
- apache tiles 2.x to 3.X

The below java code changes are as per the above framework versions migration

| Old Class/Package | New Class/Package |
|-----------------------------|-------------------------------|
| org.hibernate.Query   | org.hibernate.query.Query   |
| javax.validation.*   | jakarta.validation.* |
| org.springframework.orm.hibernate3.annotation.AnnotationSessionFactoryBean   | org.springframework.orm.hibernate5.LocalSessionFactoryBean |
| org.springframework.orm.hibernate3.HibernateTransactionManager   | org.springframework.orm.hibernate5.HibernateTransactionManager |
| org.springframework.orm.hibernate3.HibernateOptimisticLockingFailureException   | org.springframework.orm.hibernate5.HibernateOptimisticLockingFailureException |
| com.mongodb.WriteResult   | com.mongodb.client.result.UpdateResult |
| org.hibernate.engine.SessionImplementor   | org.hibernate.engine.spi.SharedSessionContractImplementor |
| org.springframework.orm.hibernate3.annotation.AnnotationSessionFactoryBean   | org.springframework.orm.hibernate5.LocalSessionFactoryBean |
| org.springframework.web.servlet.view.tiles2.SpringBeanPreparerFactory   | org.springframework.web.servlet.view.tiles3.SpringBeanPreparerFactory |
| org.springframework.web.servlet.view.tiles2.TilesView   | org.springframework.web.servlet.view.tiles3.TilesView |
| org.springframework.http.converter.json.MappingJacksonHttpMessageConverter   | org.springframework.http.converter.json.MappingJackson2HttpMessageConverter |
| LockMode   | LockOptions |
| SessionImplementor   | SharedSessionContractImplementor |

xml & jsp changes

| Old Reference | New Reference |
|-----------------------------|-------------------------------|
| mongo:mongo   | mongo:mongo-client   |
| www.springframework.org/schema/data/mongo/spring-mongo.xsd   | www.springframework.org/schema/data/mongo/spring-mongo-3.3.xsd   |
| mongo:options   | mongo:client-settings   |
| replica-set   | cluster-hosts   |
| mongo-ref   | mongo-client-ref   |
| org.springframework.web.servlet.view.tiles2.TilesConfigurer   | org.springframework.web.servlet.view.tiles3.TilesConfigurer   |
| commandName   | modelAttribute   |


