# crmeb_java

# There is an SQL injection vulnerability in the crmeb_java system (/api/admin/system/store/order/list) interface.

crmeb_java系统/api/admin/system/store/order/list接口存在sql注入的问题；

其中keywords参数存在sql注入的问题；
There is a SQL injection vulnerability with the keywords parameter.

![image](https://user-images.githubusercontent.com/59911588/221155021-a650763b-d705-4e84-a818-bfa502ebcca7.png)

![image](https://user-images.githubusercontent.com/59911588/221154258-02730c7a-3c48-4f45-8de0-b845bc8b243e.png)

com/zbkj/admin/controller/SystemWriteOffOrderController.java 
![image](https://user-images.githubusercontent.com/59911588/221154288-46c5a21d-b3fa-4509-802f-4d923be2ffc0.png)

keywords字符串拼接导致存在SQL注入；
There is an SQL injection vulnerability due to the string concatenation of the keywords.

com/zbkj/service/service/impl/StoreOrderServiceImpl.java
![image](https://user-images.githubusercontent.com/59911588/221155226-28fd55d5-3452-4bb4-9dff-84386a6ebd09.png)

