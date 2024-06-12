# Connect java to mysql by using
- Before connect to mysql, you need to open a mysql server first.
- Download [mysql](https://dev.mysql.com/downloads/installer/)
## Netbeans
1. Open project and select **Java with Ant** and press next
2. Type the name of the project and press finish
3. Download [mysql connector](https://dev.mysql.com/downloads/connector/j/) by select **Platform Independent** and choose zip file to download
4. Extract the zip file
5. Right click libraries and select add JAR/Folder and select the mysql-connector-java-x.x.x-bin.jar file
6. Connect to the server by using these code
```java
    public static void main(String args[]) {
        try {
            Connection con = DriverManager.getConnection(
                    "jdbc:mysql://localhost:3306/databaseName", "username", "password");
//replace databaseName, username and password 
            System.out.println("Connect successfully");
        } catch (Exception e) {
            System.out.println(e);
        }
    }
```
refer to: https://arc.net/l/quote/dphpisfs
