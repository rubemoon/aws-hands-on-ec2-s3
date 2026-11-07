
<p align="center">
  <a href="../../README.md"><img src="../../assets/images/step-header.png" alt="AWS Student Builder Group at UFFS Chapecó — voltar ao laboratório" width="100%" /></a>
</p>

<div align="center">
<h2>03 · Criando uma pasta no Amazon S3</h2>

<a href="../console/README.md"><img src="https://img.shields.io/badge/01-Console_AWS-374151?style=for-the-badge" alt="Console AWS"/></a>
<a href="../bucket/README.md"><img src="https://img.shields.io/badge/02-Criar_Bucket-374151?style=for-the-badge" alt="Criar Bucket"/></a>
<img src="https://img.shields.io/badge/03-Criar_Pasta-FF9900?style=for-the-badge" alt="Etapa atual"/>
<a href="../upload/README.md"><img src="https://img.shields.io/badge/04-Upload-374151?style=for-the-badge" alt="Upload"/></a>
<a href="../access/README.md"><img src="https://img.shields.io/badge/05-Acesso_Publico-374151?style=for-the-badge" alt="Acesso público"/></a>
<a href="../metadata/README.md"><img src="https://img.shields.io/badge/06-Metadados-374151?style=for-the-badge" alt="Metadados"/></a>
<a href="../delete/README.md"><img src="https://img.shields.io/badge/07-Excluir_Bucket-374151?style=for-the-badge" alt="Excluir bucket"/></a>

</div>

## Visão geral

O Amazon S3 permite organizar objetos utilizando pastas

Diferentemente de um sistema de arquivos tradicional, as pastas no S3 representam prefixos dos nomes dos objetos

Nesta etapa, vamos criar uma pasta dentro do bucket

## Instruções

### 1. Acesse seu bucket

No AWS Console, abra **S3 → Buckets**

Selecione o bucket criado na etapa anterior e acesse a aba **Objects**

### 2. Crie uma pasta

Clique em **Create folder**

![Botão para iniciar a criação de uma pasta](../../assets/images/folder-create-entry.png)

No campo **Folder name**, informe:

```text
cloud-folder
```

![Campo Folder name preenchido com cloud-folder](../../assets/images/folder-name.png)

Mantenha as demais configurações padrão e clique em **Create folder**

![Botão para confirmar a criação da pasta](../../assets/images/folder-create-submit.png)

### 3. Verifique a pasta

Após a criação, o Console retornará à aba **Objects**

A pasta `cloud-folder/` deverá aparecer na lista

Clique na pasta para confirmar que ela pode ser acessada

## Verificação

Confirme que a pasta `cloud-folder/` aparece dentro do bucket e pode ser acessada

<details>
<summary>Concluiu esta etapa? 🎉</summary>

<div align="center">

<img
  src="https://readme-typing-svg.demolab.com?font=Fira+Code&amp;weight=600&amp;size=22&amp;duration=2500&amp;pause=1000&amp;color=FF9900&amp;center=true&amp;vCenter=true&amp;width=700&amp;height=75&amp;lines=Great+job%2C+Builder!;S3+folder+created!;Ready+to+upload%3F"
  alt="S3 folder created"
/>

Sua pasta está pronta para receber arquivos

</div>

</details>

---

<table width="100%">
  <tr>
    <td><a href="../bucket/README.md"><img src="https://img.shields.io/badge/Previous-374151?style=for-the-badge" alt="Previous"/></a></td>
    <td align="right"><a href="../upload/README.md"><img src="https://img.shields.io/badge/Next-374151?style=for-the-badge" alt="Next"/></a></td>
  </tr>
</table>
