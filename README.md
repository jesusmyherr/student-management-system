# student-management-system

	<bean id="dataSource" class="com.mchange.v2.c3p0.ComboPooledDataSource">
		<!-- 注入属性 -->
		<property name="driverClass" value="com.mysql.jdbc.Driver"></property>
		<property name="jdbcUrl" value="jdbc:mysql://localhost:3306/userdb"></property>
		<property name="user" value="root"></property>
		<property name="password" value="root"></property>
	</bean>
  
  
CREATE TABLE `t_user` (
  `uid` int(11) NOT NULL AUTO_INCREMENT,
  `username` varchar(30) DEFAULT NULL,
  `password` varchar(30) DEFAULT NULL,
  KEY `uid` (`uid`)
) ENGINE=InnoDB AUTO_INCREMENT=12 DEFAULT CHARSET=utf8


CREATE TABLE `t_student` (
  `student_id` int(10) DEFAULT NULL,
  `name` varchar(30) DEFAULT NULL,
  `semester` int(10) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8
