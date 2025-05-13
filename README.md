# uplloaexcel
Upload Excel em massa

Não apenas uma, mas três dicas para implementar chamada de arquivo do Excel para cadastro ou edição em massa em um App desenvolvido em RAP - oData, no OnPremise.
Neste tutorial, pretendo listar meus favoritos, não limitando-os a utilizar outras implementações que estão disponíveis e muita gente utiliza. 

O primeiro, para mim, foi o primeiro, usando RAP + custom action UI5 - XLXS.js

Módulo XLSX

Este, reconhecidamente funciona. Já uso há vários anos em alguns dos apps que desenvolvi. Como está diponível a mais tempo, tenho mais base para falar bastante dele, e recomendar.

O desenvolvimento segue uma receita de bolo, que é encontrada no seguinte link: https://community.sap.com/t5/technology-blog-posts-by-members/excel-upload-using-rap-part-1/ba-p/13545399

A primeira parte fala como criar os objetos RAP e disponibilizar o APP. Siga os passos e crie todos os objetos necessários, que nada mais são dos que objetos necessários para gerar o APP RAP como Fiori elments.
Lembrem-se de ajustar o BDEF, como mostrado abaixo, para poder disponibilizar o método Adjust_numbes e implementar a geração automática do código ID; lembrem-se também de criar a SNRO relativa a esta numeração.
![image](https://github.com/user-attachments/assets/2b98a11d-0693-49f8-b930-e5b232abbcdd)

![image](https://github.com/user-attachments/assets/9fa8bf69-6c32-459d-8b7b-3263d26f2dc3)


O botão que chama o Excel, é desenvolvimento UI5 e precisa usar o Guide development, dentro do Vscode. Este passo é explicado na parte dois do tutorial acima.
