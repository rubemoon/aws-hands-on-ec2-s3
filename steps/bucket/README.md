
<p align="center">
  <a href="../../README.md"><img src="../../assets/images/step-header.png" alt="AWS Student Builder Group at UFFS Chapecó — voltar ao laboratório" width="100%" /></a>
</p>

<div align="center">
<h2>02 · Criando um bucket Amazon S3</h2>

<a href="../console/README.md"><img src="https://img.shields.io/badge/01-Console_AWS-374151?style=for-the-badge" alt="Console AWS"/></a>
<img src="https://img.shields.io/badge/02-Criar_Bucket-FF9900?style=for-the-badge" alt="Etapa atual"/>
<a href="../folder/README.md"><img src="https://img.shields.io/badge/03-Criar_Pasta-374151?style=for-the-badge" alt="Criar pasta"/></a>
<a href="../upload/README.md"><img src="https://img.shields.io/badge/04-Upload-374151?style=for-the-badge" alt="Upload"/></a>
<a href="../access/README.md"><img src="https://img.shields.io/badge/05-Acesso_Publico-374151?style=for-the-badge" alt="Acesso público"/></a>
<a href="../metadata/README.md"><img src="https://img.shields.io/badge/06-Metadados-374151?style=for-the-badge" alt="Metadados"/></a>
<a href="../delete/README.md"><img src="https://img.shields.io/badge/07-Excluir_Bucket-374151?style=for-the-badge" alt="Excluir bucket"/></a>

</div>

## Visão geral

O Amazon S3 é um serviço de armazenamento de objetos na nuvem

Nesta etapa, vamos criar um bucket e conhecer suas principais configurações

## Instruções

### 1. Acesse o Amazon S3

No AWS Console, pesquise por **S3** e selecione o serviço

![Resultado da busca pelo serviço Amazon S3](../../assets/images/s3-service-search.png)

No painel do S3, clique em **Create bucket**

![Botão para iniciar a criação de um bucket](../../assets/images/bucket-create-entry.png)

### 2. Escolha um nome único

Em **Bucket name**, informe um nome, por exemplo:

```text
uffs-s3-lab-123abc
```

O nome precisa ser único entre todos os buckets da mesma partição AWS. Se ele já estiver em uso, escolha outro nome acrescentando uma combinação própria de letras e números

![Nome do bucket](../../assets/images/bucket-name.png)

Se aparecer o aviso **Bucket with the same name already exists**, escolha outro nome e tente novamente

![Aviso de que o nome do bucket já existe](../../assets/images/bucket-name-already-exists.png)

O nome do bucket deve:

- Ser único entre todos os buckets da mesma partição AWS
- Ter entre 3 e 63 caracteres
- Utilizar letras minúsculas, números, pontos ou hífens
- Não ter formato de endereço IP

Confirme que a região selecionada corresponde à região definida para o laboratório

### 3. Mantenha as configurações de segurança padrão

Na seção **Object Ownership**, mantenha a opção padrão:

**ACLs disabled (recommended)**

![Opção recomendada de Object Ownership](../../assets/images/bucket-object-ownership.png)

Em **Block Public Access settings for this bucket**, mantenha:

**Block all public access** ativado

![Configuração Block all public access ativada](../../assets/images/bucket-block-public-access.png)

Essas configurações ajudam a evitar a exposição acidental de arquivos

Não altere o bloqueio de acesso público nesta etapa. As instruções do laboratório indicarão se e quando será necessário modificá-lo

### 4. Crie o bucket

Revise as configurações e clique no botão **Create bucket** no final da página

![Botão para confirmar a criação do bucket](../../assets/images/bucket-create-submit.png)

Aguarde a confirmação de que o bucket foi criado

![Confirmação de criação do bucket uffs-lab-bucket](../../assets/images/bucket-created.png)

### 5. Confira o bucket criado

Na lista de buckets, clique no nome do bucket criado

Abra a aba **Properties** para visualizar suas configurações

Nenhuma alteração é necessária por enquanto

## Verificação

Confirme que o bucket aparece na lista de buckets e que suas propriedades estão acessíveis

<details>
<summary>Concluiu esta etapa? 🎉</summary>

<div align="center">

<img
  src="https://readme-typing-svg.demolab.com?font=Fira+Code&amp;weight=600&amp;size=22&amp;duration=2500&amp;pause=1000&amp;color=569A31&amp;center=true&amp;vCenter=true&amp;width=700&amp;height=75&amp;lines=Great+job%2C+Builder!;S3+bucket+created!;Ready+for+the+next+step%3F"
  alt="S3 bucket created"
/>

Seu bucket está pronto para receber arquivos

</div>

</details>

---

<table width="100%">
  <tr>
    <td><a href="../console/README.md"><img src="https://img.shields.io/badge/Previous-374151?style=for-the-badge" alt="Previous"/></a></td>
    <td align="right"><a href="../folder/README.md"><img src="https://img.shields.io/badge/Next-374151?style=for-the-badge" alt="Next"/></a></td>
  </tr>
</table>
