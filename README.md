# 20487D_MOD03_DEMO_L2_Starter
Module 3: Creating and Consuming ASP.NET Core Web APIs

JOSE VICENTE TEJERO - 19/12/2020

RESUMEN
Creating Your First ASP.NET Core Web API

PROBLEMAS
No

 

 

 

20487D_MOD03_DEMO

 

\# Lesson 2: Creating an ASP.NET Core Web API

 

\### Demonstration: Creating Your First ASP.NET Core Web API

 

​                               ![image-20201222131631958](image-20201222131631958.png)

 

 ![image-20201222131639091](image-20201222131639091.png)

 

![image-20201222131650826](image-20201222131650826.png)

![image-20201222131658737](image-20201222131658737.png)

![image-20201222131706712](image-20201222131706712.png)

 

\# Lesson 3: Consuming ASP.NET Core Web APIs** 

 

\### **Demonstration: Consuming Services by Using JavaScript**



![image-20201222131723223](image-20201222131723223.png)

![image-20201222131730853](C:\Users\josev\AppData\Roaming\Typora\typora-user-images\image-20201222131730853.png)

![image-20201222131739834](image-20201222131739834.png)



![image-20201222131747052](image-20201222131747052.png)

**Demonstration: Consuming Services by Using HttpClient**



![image-20201222131800724](image-20201222131800724.png)

![image-20201222131807426](image-20201222131807426.png)

![image-20201222131814844](image-20201222131814844.png)

![image-20201222131820850](image-20201222131820850.png)

**# Lesson 4: Handling HTTP Requests and Responses**

**### Demonstration: Throwing Exceptions**

![image-20201222131831375](image-20201222131831375.png)

![image-20201222131839728](image-20201222131839728.png)

**# Lesson 5: Automatically Generating HTTP Requests and Responses**

 

**### Demonstration: Testing HTTP requests with Swagger**



![image-20201222131853506](image-20201222131853506.png)



![image-20201222131902373](image-20201222131902373.png)



**Demonstration: Generating C# HTTP Clients by Using AutoRest**



![image-20201222131919705](image-20201222131919705.png)

![image-20201222131924829](image-20201222131924829.png)

Instalamos la última versión de autorest y le damos autorest --rest

![image-20201222131936294](image-20201222131936294.png)

![image-20201222131945216](image-20201222131945216.png)

A partir del fichero json:

https://localhost:5001/swagger/v1/swagger.json

Se obtiene el .jaml o directamente:

 

Alternativa al yaml

autorest -Input http://localhost:5000/swagger/v1/swagger.json -CodeGenerator CSharp -Namespace AutoRest.Sdk

o con yaml:

 autorest --input-file="http://localhost:5000/swagger/v1/swagger.json" --csharp --output --namespace=Autorest.sdk

 

Finalmente se obtiene generated.

![image-20201222132013863](image-20201222132013863.png)

![image-20201222132020419](image-20201222132020419.png)

![image-20201222132027641](image-20201222132027641.png)
