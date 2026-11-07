<p align="center">
  <a href="../../README.md"><img src="../../assets/images/step-header.png" alt="AWS Student Builder Group at UFFS Chapecó — voltar ao laboratório" width="100%" /></a>
</p>

<div align="center">

<h2>06 · Gerenciando metadados no Amazon S3</h2>

<a href="../console/README.md"><img src="https://img.shields.io/badge/01-Console_AWS-374151?style=for-the-badge" alt="Console AWS"/></a>
<a href="../bucket/README.md"><img src="https://img.shields.io/badge/02-Criar_Bucket-374151?style=for-the-badge" alt="Criar bucket"/></a>
<a href="../folder/README.md"><img src="https://img.shields.io/badge/03-Criar_Pasta-374151?style=for-the-badge" alt="Criar pasta"/></a>
<a href="../upload/README.md"><img src="https://img.shields.io/badge/04-Upload-374151?style=for-the-badge" alt="Upload"/></a>
<a href="../access/README.md"><img src="https://img.shields.io/badge/05-Acesso_Publico-374151?style=for-the-badge" alt="Acesso público"/></a>
<img src="https://img.shields.io/badge/06-Metadados-FF9900?style=for-the-badge" alt="Etapa atual"/>
<a href="../delete/README.md"><img src="https://img.shields.io/badge/07-Excluir_Bucket-374151?style=for-the-badge" alt="Excluir bucket"/></a>

</div>

## Visão geral

Os metadados do Amazon S3 são informações armazenadas como pares de chave e valor e ajudam a descrever os objetos

Nesta etapa, vamos reenviar o arquivo de teste com metadados de sistema e uma informação personalizada

> Esta etapa substitui o objeto de teste enviado anteriormente. Mantenha uma cópia local do arquivo antes de removê-lo

## Instruções

### 1. Remova o objeto de teste

No Amazon S3, abra seu bucket e acesse `cloud-folder/`

Selecione somente o arquivo de teste usado nas etapas anteriores e clique em **Delete**

![Arquivo de teste selecionado](../../assets/images/metadata-object-selected.png)

![Botão Delete do objeto selecionado](../../assets/images/metadata-delete-button.png)

Na tela de confirmação, digite `permanently delete`

![Campo de confirmação de exclusão](../../assets/images/metadata-delete-confirmation.png)

Clique em **Delete objects** para confirmar

![Botão Delete objects](../../assets/images/metadata-delete-objects-button.png)

> Exclua somente o objeto de teste. Não exclua o bucket nem outros arquivos

### 2. Envie o arquivo novamente

Retorne à pasta `cloud-folder/` e inicie um upload

Clique em **Upload → Add files** e selecione a cópia local do mesmo arquivo

Antes de concluir o upload, localize a seção **Properties → Metadata**

### 3. Configure os metadados

Clique em **Add metadata**

![Botão Add metadata](../../assets/images/metadata-add-button.png)

Em **System defined**, selecione **Content-Type**

Use um tipo de conteúdo que corresponda ao arquivo:

- Para a imagem PNG deste laboratório, use `image/png`
- Use `text/plain` somente para um arquivo de texto

A captura de exemplo mostra `text/plain`; não use esse valor para uma imagem PNG

![Exemplo de metadado Content-Type no formulário de upload](../../assets/images/metadata-system-defined.png)

Clique em **Add metadata** para adicionar um registro personalizado

Em **Type**, selecione **User defined** e informe a chave e o valor:

| Campo | Valor |
|---|---|
| Key | `x-amz-meta-image-type` |
| Value | `logo` |

![Metadado personalizado definido pelo usuário](../../assets/images/metadata-user-defined.png)

O prefixo `x-amz-meta-` identifica metadados definidos pelo usuário no Amazon S3

### 4. Conclua o upload

Confira o nome do arquivo e os metadados. Clique em **Upload** e aguarde a confirmação

![Botão Upload](../../assets/images/upload-submit-button.png)

Depois, selecione **Close** e abra o objeto enviado

## Verificação

Na página do objeto, abra **Properties → Metadata**

Confirme que os metadados estão associados ao objeto. O `Content-Type` esperado depende do arquivo enviado; a captura mostra `text/plain` como exemplo

![Exemplo de metadados do objeto](../../assets/images/metadata-result.png)

O objeto permanece privado, a menos que uma política ou outra configuração permita acesso público

<details>
<summary>Concluiu esta etapa? 🎉</summary>

<div align="center">

<img
  src="https://readme-typing-svg.demolab.com?font=Fira+Code&amp;weight=600&amp;size=22&amp;duration=2500&amp;pause=1000&amp;color=FF9900&amp;center=true&amp;vCenter=true&amp;width=700&amp;height=75&amp;lines=Excellent+work%2C+Builder!;S3+metadata+configured!;One+last+mission+to+go!"
  alt="S3 metadata completed"
/>

Você configurou metadados de sistema e personalizados no Amazon S3

</div>

</details>

---

<table width="100%">
  <tr>
    <td><a href="../access/README.md"><img src="https://img.shields.io/badge/Previous-374151?style=for-the-badge" alt="Previous"/></a></td>
    <td align="right"><a href="../delete/README.md"><img src="https://img.shields.io/badge/Next-374151?style=for-the-badge" alt="Next"/></a></td>
  </tr>
</table>
