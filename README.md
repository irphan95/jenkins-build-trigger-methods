# jenkins-build-trigger-methods
1. ## POLL SCM:
- ##### Click on the new item option
![step1](https://user-images.githubusercontent.com/103019032/187117412-7807dbbd-1eb8-4533-8621-c8b3d489595b.PNG)
- #### After clicking on new item, the new interface will open,and type the project name,and also type of project,now i have choosed free style project.
![image](https://user-images.githubusercontent.com/103019032/187118008-86914868-0d0f-46c2-92cc-18a8da577752.png)
- #### After that,in a general option,i have type description,its optional.
![step3](https://user-images.githubusercontent.com/103019032/187119009-e5021da4-f6f1-402a-aba4-42743dbbfec6.PNG)
- #### The next option is, source code management,in git option,from where we will get our code,if your repository is private,then you need to credentials,otherwise no need to credential.
![step4](https://user-images.githubusercontent.com/103019032/187119519-36d4ca4a-f905-4199-bf43-70f8545dddc3.PNG)
- #### In a build trigger method,i'have select poll scm option with cron,it means for example cron have * * * * *(in a left side * means minute,the next * means hours, the next * means day, the next * means month, and the next * means year),so i have taken H/2 * * * *,it means if i will any changes in git repository,it automatically build every 2 minutes.
![step5](https://user-images.githubusercontent.com/103019032/187120322-82006998-fb9d-4eb7-8989-ac311cd53c16.PNG)
- ####  The next option is build environment,I have left this as default.
![step6](https://user-images.githubusercontent.com/103019032/187120577-ab285800-3710-4019-ab4c-ea48738c873b.PNG)
- #### The next option is build environment,so i have choose execute shell option,and tyle the ls,pwd, and running the python program.
![step7](https://user-images.githubusercontent.com/103019032/187121292-c36db297-85c6-4b05-93fa-a82be4b30ea5.PNG)


