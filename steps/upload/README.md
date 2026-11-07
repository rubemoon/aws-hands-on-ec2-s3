
<p align="center">
  <a href="../../README.md"><img src="../../assets/images/step-header.png" alt="AWS Student Builder Group at UFFS Chapecó — voltar ao laboratório" width="100%" /></a>
</p>

<div align="center">
<h2>04 · Enviando arquivos para o Amazon S3</h2>

<a href="../console/README.md"><img src="https://img.shields.io/badge/01-Console_AWS-374151?style=for-the-badge" alt="Console AWS"/></a>
<a href="../bucket/README.md"><img src="https://img.shields.io/badge/02-Criar_Bucket-374151?style=for-the-badge" alt="Criar bucket"/></a>
<a href="../folder/README.md"><img src="https://img.shields.io/badge/03-Criar_Pasta-374151?style=for-the-badge" alt="Criar pasta"/></a>
<img src="https://img.shields.io/badge/04-Upload-FF9900?style=for-the-badge" alt="Etapa atual"/>
<a href="../access/README.md"><img src="https://img.shields.io/badge/05-Acesso_Publico-374151?style=for-the-badge" alt="Acesso público"/></a>
<a href="../metadata/README.md"><img src="https://img.shields.io/badge/06-Metadados-374151?style=for-the-badge" alt="Metadados"/></a>
<a href="../delete/README.md"><img src="https://img.shields.io/badge/07-Excluir_Bucket-374151?style=for-the-badge" alt="Excluir bucket"/></a>

</div>

## Visão geral

O Amazon S3 armazena arquivos como objetos, identificados por uma chave dentro de um bucket

Nesta etapa, vamos enviar um arquivo de teste para a pasta criada anteriormente

## Instruções

### 1. Abra a pasta

No Amazon S3, acesse seu bucket e clique em `cloud-folder/`

Confira o caminho de navegação para confirmar que está dentro do bucket e da pasta corretos

![Caminho do bucket e da pasta cloud-folder](../../assets/images/upload-folder-breadcrumb.png)

### 2. Adicione um arquivo

Dentro da pasta, clique em **Upload**

![Botão Upload dentro da pasta](../../assets/images/upload-button.png)

Na página de envio, clique em **Add files** e selecione um arquivo de teste no seu computador

![Botão Add files](../../assets/images/upload-add-files-button.png)

Confirme que o arquivo aparece na lista **Files and folders**

![Arquivo selecionado para upload](../../assets/images/upload-files-list.png)

Se necessário, marque a caixa ao lado do arquivo para selecioná-lo. O botão **Remove** serve para retirar um arquivo da lista antes do envio

![Arquivo marcado na lista](../../assets/images/upload-file-selected.png)

![Botão Remove para retirar um arquivo da lista](../../assets/images/upload-remove-button.png)

### 3. Envie o arquivo

Clique em **Upload** e aguarde a mensagem de confirmação

![Botão Upload para confirmar o envio](../../assets/images/upload-submit-button.png)

![Confirmação de upload concluído](../../assets/images/upload-success.png)

Clique em **Close** para retornar à pasta

![Botão Close](../../assets/images/upload-close-button.png)

## Verificação

Abra `cloud-folder/` e confirme que o arquivo aparece na aba **Files and folders**

![Arquivo armazenado dentro de cloud-folder](../../assets/images/upload-object.png)

O caminho do objeto terá este formato

```text
s3://nome-do-bucket/cloud-folder/nome-do-arquivo
```

<details>
<summary>Concluiu esta etapa? 🎉</summary>

<div align="center">

<img
  src="https://readme-typing-svg.demolab.com?font=Fira+Code&amp;weight=600&amp;size=22&amp;duration=2500&amp;pause=1000&amp;color=FF9900&amp;center=true&amp;vCenter=true&amp;width=700&amp;height=75&amp;lines=Great+job%2C+Builder!;File+uploaded+successfully!;Ready+for+the+next+mission%3F"
  alt="S3 upload completed"
/>

Seu arquivo está armazenado no Amazon S3

</div>

</details>

---

<table width="100%">
  <tr>
    <td><a href="../folder/README.md"><img src="https://img.shields.io/badge/Previous-374151?style=for-the-badge" alt="Previous"/></a></td>
    <td align="right"><a href="../access/README.md"><img src="https://img.shields.io/badge/Next-374151?style=for-the-badge" alt="Next"/></a></td>
  </tr>
</table>
