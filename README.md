# BudgetApplication07:48:04,785 INFO  [org.hibernate.dialect.Dialect] (ServerService Thread Pool -- 87) HHH000400: Using dialect: org.hibernate.dialect.DB2Dialect
07:48:05,741 ERROR [org.hibernate.engine.jdbc.env.internal.JdbcEnvironmentImpl] (ServerService Thread Pool -- 87) Could not fetch the SequenceInformation from the database: com.ibm.db2.jcc.am.SqlSyntaxErrorException: SYSCAT.SEQUENCES IS AN UNDEFINED NAME. SQLCODE=-204, SQLSTATE=42704, DRIVER=4.16.53
        at com.ibm.db2.jcc.am.fd.a(fd.java:739)
        at com.ibm.db2.jcc.am.fd.a(fd.java:60)
        at com.ibm.db2.jcc.am.fd.a(fd.java:127)
        at com.ibm.db2.jcc.am.to.c(to.java:2771)
        at com.ibm.db2.jcc.am.to.d(to.java:2759)
        at com.ibm.db2.jcc.am.to.a(to.java:2192)
        at com.ibm.db2.jcc.am.to.a(to.java:2168)
        at com.ibm.db2.jcc.t4.ab.h(ab.java:136)

EntityManagerFactory for persistence unit 'tccsPU'
07:48:07,571 ERROR [org.springframework.web.servlet.DispatcherServlet] (ServerService Thread Pool -- 87) Context initialization failed: org.springframework.beans.factory.UnsatisfiedDependencyException: Error creating bean with name 'messageListener': Unsatisfied dependency expressed through field 'messageSender'; nested exception is org.springframework.beans.factory.UnsatisfiedDependencyException: Error creating bean with name 'messageSender': Unsatisfied dependency expressed through field 'jmsTemplate'; nested exception is org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'jmsTemplate' defined in gov.irs.tccs.messaging.MessagingConfiguration: Bean instantiation via factory method failed; nested exception is org.springframework.beans.BeanInstantiationException: Failed to instantiate [org.springframework.jms.core.JmsTemplate]: Factory method 'jmsTemplate' threw exception; nested exception is org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'cachingConnectionFactory' defined in gov.irs.tccs.messaging.MessagingConfiguration: Post-processing of merged bean definition failed; nested exception is java.lang.IllegalStateException: Failed to introspect Class [org.springframework.jms.connection.SingleConnectionFactory] from ClassLoader [ModuleClassLoader for Module "deployment.fis-tccs-1.4.war" from Service Module Loader]
        at org.springframework.beans.factory.annotation.AutowiredAnnotationBeanPostProcessor$AutowiredFieldElement.resolveFieldValue(AutowiredAnnotationBeanPostProcessor.java:659)
        at org.springframework.beans.factory.annotation.AutowiredAnnotationBeanPostProcessor$AutowiredFieldElement.inject(AutowiredAnnotationBeanPostProcessor.java:639)
        at org.springframework.beans.factory.annotation.InjectionMetadata.inject(InjectionMetadata.java:119)
        at org.springframework.beans.factory.annotation.AutowiredAnnotationBeanPostProcessor.postProcessProperties(AutowiredAnnotationBeanPostProcessor.java:399)
        at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.populateBean(AbstractAutowireCapableBeanFactory.java:1431)
        at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.doCreateBean(AbstractAutowireCapableBeanFactory.java:619)
        at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.createBean(AbstractAutowireCapableBeanFactory.java:542)
        at org.springframework.beans.factory.support.AbstractBeanFactory.lambda$doGetBean$0(AbstractBeanFactory.java:335)
        at org.springframework.beans.factory.support.DefaultSingletonBeanRegistry.getSingleton(DefaultSingletonBeanRegistry.java:234)
        at org.springframework.beans.factory.support.AbstractBeanFactory.doGetBean(AbstractBeanFactory.java:333)
        at org.springframework.beans.factory.support.AbstractBeanFactory.getBean(AbstractBeanFactory.java:208)
        at org.springframework.beans.factory.support.DefaultListableBeanFactory.preInstantiateSingletons(DefaultListableBeanFactory.java:953)
      
        
