# Simple-pipeline-with-CodeCommit-CodeDeploy-EC2

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/32c5f0ea-0781-40b7-a01c-d47b2469bdd0)

### We will deploy this website using codeploy

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/59783049-bcaf-464c-9fcd-d8247e4ce2bc)


### We will modify the html file and trigger aws pipeline for new website

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/e215e25f-39d3-47ee-bc6e-a417bf05f9ce)

# 1-create CodeCommit repository

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/efb4aca6-3869-453a-bda3-2cbd49b1ac97)

# 2-Clone https in Cloud9IDE

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/8117ecd9-33f3-4a7d-a8cd-696f16864bc9)

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/0b5f5069-e624-489a-ae54-e71951181caf)

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/0650ebcf-e4d8-454e-a80b-9563440e6e62)

Execute those command in MyDemoRepo(Master) Cloud9

Ajouter les fichiers qui seront inclus dans le prochain index: $ git add -A

Enregistrer les modifications dans l’historique de git: $ git commit -m "Add sample application file"

Envoyer ces modifications sur le dépôt distant avec : $ git push

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/7662451f-57c8-4635-8f7d-623bfd9eb80e)

# 3-CodeDeploy

Create Ec2 where we are going the sample of application and Install CodeDeploy agent on EC2 to be part of CodeDeploy group


# 4-Create role for Ec2, codedeploy and CodeDeployement group

## Create role for Ec2 and create EC2

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/092744fe-3eca-4133-97f0-0411a249eb45)

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/1c7926e1-d639-438f-92b3-d7de7fbd12e7)

## Create role for codedeploy and CodeDeployement group

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/95f10d87-bf74-4c43-94a2-991252b12ab6)

Create Codedeploy application

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/a7d3b527-e00b-40da-ada9-f562b54a3663)

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/5fa9e908-c66f-4717-a24f-bba2e650e3c3)


# 5-Create Pipelene

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/00aea403-2300-44bc-adfe-92cbc2ee1e6d)

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/6c42da52-b4fd-4469-87ab-36a542e67d68)

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/c48737ab-13e3-42b1-a0c0-ba806d923f1f)

## Copy the public ip DNS and paste in

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/a9f8498d-7817-4045-958d-ace5fba4db5f)

![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/75c2378b-5484-4d14-ac79-33af7baff1e3)

# If we make change in Cloud9 every thing will change in the web page

For example make the change of index.html code and commit the change


```py
<!DOCTYPE html>
<html>
<head>
  <title>Updated Sample Deployment</title>
  <style>
    body {
      color: #000000;
      background-color: #CCFFCC;
      font-family: Arial, sans-serif;  
      font-size:14px;
    }
        
    h1 {
      font-size: 250%;
      font-weight: normal;
      margin-bottom: 0;
    }
    
    h2 {
      font-size: 175%;
      font-weight: normal;
      margin-bottom: 0;
    }
  </style>
</head>
<body>
  <div align="center"><h1>Updated Sample Deployment</h1></div>
  <div align="center"><h2>This application was updated using CodePipeline, CodeCommit, and CodeDeploy.</h2></div>
  <div align="center">
    <p>Learn more:</p> 
    <p><a href="https://docs.aws.amazon.com/codepipeline/latest/userguide/">CodePipeline User Guide</a></p>
    <p><a href="https://docs.aws.amazon.com/codecommit/latest/userguide/">CodeCommit User Guide</a></p>
    <p><a href="https://docs.aws.amazon.com/codedeploy/latest/userguide/">CodeDeploy User Guide</a></p>
  </div>
</body>
</html>
```


![image](https://github.com/felixdagnon/demo-simple-pipeline/assets/91665833/e253889c-38ad-42f2-ad32-6f0f04da9db7)












































