
<p align="center">
  <a href="../../README.md"><img src="../../assets/images/step-header.png" alt="AWS Student Builder Group at UFFS Chapecó — voltar ao laboratório" width="100%" /></a>
</p>

<div align="center">
<h2>07 · Excluindo um bucket S3</h2>

<a href="../console/README.md"><img src="https://img.shields.io/badge/01-Console_AWS-374151?style=for-the-badge" alt="Console AWS"/></a>
<a href="../bucket/README.md"><img src="https://img.shields.io/badge/02-Criar_Bucket-374151?style=for-the-badge" alt="Criar bucket"/></a>
<a href="../folder/README.md"><img src="https://img.shields.io/badge/03-Criar_Pasta-374151?style=for-the-badge" alt="Criar pasta"/></a>
<a href="../upload/README.md"><img src="https://img.shields.io/badge/04-Upload-374151?style=for-the-badge" alt="Upload"/></a>
<a href="../access/README.md"><img src="https://img.shields.io/badge/05-Acesso_Publico-374151?style=for-the-badge" alt="Acesso público"/></a>
<a href="../metadata/README.md"><img src="https://img.shields.io/badge/06-Metadados-374151?style=for-the-badge" alt="Metadados"/></a>
<img src="https://img.shields.io/badge/07-Excluir_Bucket-FF9900?style=for-the-badge" alt="Etapa atual"/>

</div>

## Visão geral

O Amazon S3 permite excluir buckets e seus objetos quando não são mais necessários

Nesta etapa, vamos esvaziar e excluir somente o bucket criado durante o laboratório

> **Atenção:** esta operação é destrutiva e não pode ser desfeita. Confirme cuidadosamente o nome do bucket e verifique que não há arquivos importantes antes de continuar

## Instruções

### 1. Localize o bucket

No AWS Management Console, pesquise por **S3** e abra o serviço

![Atalho do serviço Amazon S3](../../assets/images/delete-s3-service-menu.png)

Na página **Buckets**, selecione o bucket criado anteriormente

![Navegação para a página Buckets](../../assets/images/delete-buckets-breadcrumb.png)

Confira o nome do bucket selecionado antes de prosseguir

![Bucket de laboratório selecionado](../../assets/images/delete-bucket-selected.png)

### 2. Esvazie o bucket

Com o bucket selecionado, clique em **Empty**

![Botão Empty](../../assets/images/delete-empty-button.png)

Na tela de confirmação, digite:

```text
permanently delete
```

![Campo de confirmação do esvaziamento](../../assets/images/delete-empty-confirmation.png)

Clique em **Empty** para confirmar a exclusão dos objetos

![Botão para confirmar o esvaziamento](../../assets/images/delete-empty-submit-button.png)

Aguarde a confirmação de que o bucket foi esvaziado

![Confirmação de que o bucket foi esvaziado](../../assets/images/delete-empty-success.png)

Clique em **Exit** para retornar à lista de buckets

![Botão Exit](../../assets/images/delete-empty-exit-button.png)

### 3. Exclua o bucket

Selecione novamente o bucket vazio e clique em **Delete**

![Botão Delete do bucket](../../assets/images/delete-bucket-button.png)

Na tela de confirmação, digite o **nome exato do seu bucket**

![Campo de confirmação com o nome do bucket](../../assets/images/delete-bucket-confirmation.png)

Confira o nome digitado e clique em **Delete bucket** para finalizar

![Confirmação de que o bucket foi excluído](../../assets/images/delete-bucket-success.png)

> Após a exclusão, o nome do bucket poderá ser utilizado por outra conta AWS

## Verificação

Retorne à página **Buckets** e confirme que o bucket excluído não aparece mais na lista

Se a exclusão falhar, confirme que todos os objetos foram removidos e que você selecionou o bucket correto

<details>
<summary>Concluiu o laboratório? 🎉</summary>

<div align="center">

<img
  src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=23&duration=2500&pause=1000&color=FF9900&center=true&vCenter=true&width=750&height=85&lines=Congratulations%2C+Builder!;Amazon+S3+Lab+Completed!;Keep+Building.+Keep+Exploring."
  alt="Amazon S3 Lab Completed"
/>

<h3>Mission accomplished!</h3>

Você concluiu o laboratório Amazon S3 e explorou a criação de buckets, organização de objetos, upload de arquivos, permissões, metadados e exclusão de recursos

<p>
  <a href="https://github.com/rubemoon/aws-hands-on-ec2-s3/tree/challenge">
    <img src="https://img.shields.io/badge/Next%20Mission-Challenge-8957E5?style=for-the-badge" alt="Next Mission: Challenge"/>
  </a>
</p>

</div>

</details>

---

<table width="100%">
  <tr>
    <td><a href="../metadata/README.md"><img src="https://img.shields.io/badge/Previous-374151?style=for-the-badge" alt="Previous"/></a></td>
    <td align="right"></td>
  </tr>
</table>
