### Lambda Function de Start/Stop de instancias EC2
        Função Lambda para schedular um stop e um start em instancias do ec2 de forma automatizada utilizando uma integração com o CloudWatch.

#### Necessário criar uma ou mais instancias ec2 free tier(micro) a fim de testes.
![](/imagens/1.PNG) 

#### Criar uma nova política a partir de um JSON na parte de IAM

![](/imagens/5.PNG)

#### Criar uma role com essa política, e com a política de execução de nossa função LAMBDA que vamos criar.

![](/imagens/6.PNG)

#### Criar nossa função lambda

![](/imagens/2.PNG)

![](/imagens/3.PNG)

![](/imagens/4.PNG)

#### Cria duas regras de START  e STOP no cloudwatch

![](/imagens/7.PNG)

#### Criar um crontab específico para cada regra

![Start](/imagens/8.PNG)

![Stop](/imagens/9.PNG)

#### Por fim colocar a tag que decidimos no cloudwatch event nas tags das instancias.

![](/imagens/Capture.PNG)