# jenkins-build-trigger-methods
## 1.POLL SCM:
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
![step9](https://user-images.githubusercontent.com/103019032/187125471-c01dd4a7-15fa-4e59-a992-995e891e7c4a.PNG)
- #### the next option is post build actions so I have left this as default.
![step8](https://user-images.githubusercontent.com/103019032/187121818-0c8592bd-5111-4dfe-a5b6-8a2fcb1577a1.PNG)
- #### Now i have some changes in github repository,and commit for changes.
![image](https://user-images.githubusercontent.com/103019032/187126072-fcdd0183-638b-45fa-9554-e69c3df36be8.png)
- #### After change in github repository,jenkins automatically build again after 2 minutes.
![image](https://user-images.githubusercontent.com/103019032/187127110-c6094f1a-19d3-4beb-8fa0-7619b89095bb.png)


## 2. Trigger build remotely

- ##### Click on the new item option
![step1](https://user-images.githubusercontent.com/103019032/187135741-fbc54842-4efc-4d76-971d-669bef529771.PNG)
- #### After clicking on new item, the new interface will open,and type the project name,and also type of project,now i have choosed free style project.
![step2](https://user-images.githubusercontent.com/103019032/187136069-823e52ac-2d33-4683-bad7-9c1a7cb11828.PNG)
- #### After this step, In general option you can choose option according to your need or leave it.
![step3](https://user-images.githubusercontent.com/103019032/187136851-929d7cb5-e1fb-4423-8fa9-44021ce489c6.PNG)
- #### The next option is, source code management,in git option,from where we will get our code,if your repository is private,then you need to credentials,otherwise no need to credential.
![step4](https://user-images.githubusercontent.com/103019032/187139042-a687fcc3-e748-493e-baa8-b1834361b039.PNG)
- ####  In a build trigger method,i'have select trigger builds remotely option, Trigger builds Remotely” feature provides flexibility that allows triggering a job from the script, command line, GitHub hook when somebody has committed a change or triggers a job from one server to another.In this, we can see JENKINS_URL/job/jenkins-builds-remotely/build?token=TOKEN_NAME.
![step5](https://user-images.githubusercontent.com/103019032/187140619-8669f918-4eb5-4813-b5a3-0df376dc902c.PNG)
- #### The next option is build environment,so i have choose execute shell option,and tyle the ls,pwd, and running the python program.
 ![step6](https://user-images.githubusercontent.com/103019032/187140793-76125ae2-5015-4c3f-8c39-15e4477945d8.PNG)
- #### the next option is post build actions so I have left this as default.
![step7](https://user-images.githubusercontent.com/103019032/187141118-11b56e8c-9a26-4073-8700-c9ed4e129f28.PNG)
- #### Now we can build remotely using this https://192.168.6.234/job/jenkins-builds-remotely/build?token=my-token 
![step8](https://user-images.githubusercontent.com/103019032/187142265-5687d2b2-d4b2-4875-8266-6164f19f7a2b.PNG)
- #### Now we can check in console output
![step9](https://user-images.githubusercontent.com/103019032/187142398-bc2eb783-ee98-4760-874e-55a54b655a27.PNG)














