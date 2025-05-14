# uplloaexcel
Upload Excel em massa

Não apenas uma, mas três dicas para implementar chamada de arquivo do Excel para cadastro ou edição em massa em um App desenvolvido em RAP - oData, no OnPremise.
Neste tutorial, pretendo listar meus favoritos, não limitando-os a utilizar outras implementações que estão disponíveis e muita gente utiliza. 

O primeiro, para mim, foi o primeiro, usando RAP + custom action UI5 - XLXS.js

Módulo XLSX

Este, reconhecidamente funciona. Já uso há vários anos em alguns dos apps que desenvolvi. Como está diponível a mais tempo, tenho mais base para falar bastante dele, e recomendar.

O desenvolvimento segue uma receita de bolo, que é encontrada no seguinte link: https://community.sap.com/t5/technology-blog-posts-by-members/excel-upload-using-rap-part-1/ba-p/13545399

A primeira parte fala como criar os objetos RAP e disponibilizar o APP, Creating an OData Service using SAP RAP Model. Siga os passos e crie todos os objetos necessários, que nada mais são dos que objetos necessários para gerar o APP RAP como Fiori elments.
Lembrem-se de ajustar o BDEF, como mostrado abaixo, para poder disponibilizar o método Adjust_numbes e implementar a geração automática do código ID; lembrem-se também de criar a SNRO relativa a esta numeração.

![image](https://github.com/user-attachments/assets/2b98a11d-0693-49f8-b930-e5b232abbcdd)

![image](https://github.com/user-attachments/assets/9fa8bf69-6c32-459d-8b7b-3263d26f2dc3)


A segunda parte fala como Extender o app Fiori elements com a funcionanlidade do upload.
Para isso, siga os passos e utilize o Guided Development para implementar o botão e customize o fragment (diálogo que mostrará quando clicar no botão upload excel). Para que já está acostumado utilizar o Guided development, é bem simples. Para que não está, siga os passos e veja qual simples é.
Ao final da parte 2, já temos como abrir o diálogo do upload excel através do custom button criado.

![image](https://github.com/user-attachments/assets/8e02a705-4bee-48cf-9a21-0ec2f1cab71a)


O passo três fala de como instalar o módulo e cofigurar para subir junto no deploy. 

Dica: Pode utilizar o XLSX.js dentro da pasta ext, com isso você elimina a parte de precisar configurar os arquivos .yaml.

![image](https://github.com/user-attachments/assets/8f90ecd2-24ac-4817-b14c-521d12eb067e)

Arquivo disponível no link:

Resultado:
Upload Excel 1 - Watch Video



