This is my fixed for DPLM-3
For any questions - Please email me at DevOps@RajeshKumar.xyz
# ========================NEXUS==============================

<distributionManagement>
	<repository>
		<id>cts</id>
		<name>pavan-test</name>
		<url>http://52.66.212.86:8081/repository/pavan-test/</url>
	</repository>
 
	<snapshotRepository>
		<id>cts</id>
		<name>pavan-test2</name>
		<url>http://52.66.212.86:8081/repository/pavan-test2/</url>
	</snapshotRepository>

</distributionManagement>


===============ARTIFACTORY=================
<distributionManagement>
	<repository>
		<id>rajesh</id>
		<name>Internal Releases</name>
		<url>http://13.127.94.210:8081/artifactory/list/rajesh-release/</url>
	</repository>
 
	<snapshotRepository>
		<id>rajesh</id>
		<name>Internal Releases</name>
		<url>http://13.127.94.210:8081/artifactory/list/rajesh-snapshot/</url>
	</snapshotRepository>

</distributionManagement>

=====================SETTING.XML=================================
   <server>
		<id>cts</id>
		<username>admin</username>
		<password>admin123</password>
</server>

=======================Setting.xml with Artifactory Setup======================
<mirror>
      <id>central</id>
      <name>Maven Repository Manager running on repo.mycompany.com</name>
      <url>http://13.127.94.210:8081/artifactory/list/group/</url>
      <mirrorOf>*</mirrorOf>
    </mirror>
    
    

