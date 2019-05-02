# jpa-hibernate

File  for JPA Hibernate :

<persistence xmlns="http://java.sun.com/xml/ns/persistence"
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xsi:schemaLocation="http://java.sun.com/xml/ns/persistence http://java.sun.com/xml/ns/persistence/persistence_2_0.xsd"
        version="2.0">
    <persistence-unit name="EmployeeService" transaction-type="RESOURCE_LOCAL">
        <class>com.soft.infg.model.Employee</class>
        <validation-mode>NONE</validation-mode>
		<properties>
            <property name="javax.persistence.jdbc.driver" value="oracle.jdbc.driver.OracleDriver"/>
            <property name="javax.persistence.jdbc.url" value="jdbc:oracle:thin:@127.0.0.1:1521:XE"/>
            <property name="javax.persistence.jdbc.user" value="JPA"/>
            <property name="javax.persistence.jdbc.password" value="jpa"/>
           <property name="hibernate.hbm2ddl.auto" value="create-drop" />
        </properties>
    </persistence-unit>
</persistence>
