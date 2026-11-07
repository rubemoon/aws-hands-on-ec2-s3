
<p align="center">
  <a href="../../README.md"><img src="../../assets/images/step-header.png" alt="AWS Student Builder Group at UFFS Chapecó — voltar ao laboratório" width="100%" /></a>
</p>

<div align="center">

<h2>02 · Criando uma instância EC2</h2>

<a href="../console/README.md"><img src="https://img.shields.io/badge/01-Console_AWS-374151?style=for-the-badge" alt="Console AWS"/></a>
<img src="https://img.shields.io/badge/02-Criar_EC2-FF9900?style=for-the-badge" alt="Etapa atual"/>
<a href="../connect/README.md"><img src="https://img.shields.io/badge/03-Conectar_EC2-374151?style=for-the-badge" alt="Conectar à EC2"/></a>
<a href="../metadata/README.md"><img src="https://img.shields.io/badge/04-Metadados-374151?style=for-the-badge" alt="Metadados"/></a>
<a href="../terminate/README.md"><img src="https://img.shields.io/badge/05-Encerrar-374151?style=for-the-badge" alt="Encerrar"/></a>

</div>

## Visão geral

O Amazon EC2 permite criar servidores virtuais na nuvem

Nesta etapa, vamos configurar e iniciar uma instância Linux usando o AWS Management Console

## Instruções

### 1. Acesse o Amazon EC2

No console AWS, use a busca para localizar **EC2** ou clique no atalho do serviço, quando estiver disponível

![Atalho para o serviço EC2](../../assets/images/launch-ec2.png)

No painel do EC2, clique em **Launch instance**

![Botão Launch instance](../../assets/images/launch-instance-button.png)

### 2. Configure a instância

Em **Name and tags**, informe um nome para identificar seu servidor, se desejar

Na seção **Application and OS Images**, selecione **Amazon Linux 2023**

Em **Instance type**, escolha **t3.micro**, conforme o laboratório de referência

![Selecionar Amazon Linux 2023](../../assets/images/launch-ami.png)

![Selecionar o tipo de instância t3.micro](../../assets/images/launch-instance-type.png)

### 3. Crie o par de chaves

Em **Key pair**, clique em **Create new key pair**

Em **Key pair name**, informe:

`lab-uffs-key`

Selecione o formato `.pem` para acesso SSH e clique em **Create key pair**

![Nome do par de chaves](../../assets/images/launch-keypair-name.png)

![Criar o par de chaves](../../assets/images/launch-keypair-create.png)

O navegador fará o download de `lab-uffs-key.pem`. Guarde o arquivo em local seguro. Não copie o conteúdo da chave privada para o README, mensagens ou GitHub

### 4. Configure a rede e o armazenamento

Na seção **Network settings**, verifique as configurações de rede da instância

Para conexões SSH externas, utilize a porta **22** e restrinja a origem a **My IP** sempre que possível

![Configuração de acesso SSH](../../assets/images/launch-ssh-setting.png)

As capturas seguintes mostram a opção **Anywhere** (`0.0.0.0/0`) e o aviso de segurança exibido pela AWS. Essa configuração permite tentativas de conexão de qualquer endereço IP; use-a somente se as instruções do laboratório exigirem e pelo menor tempo possível

![Aviso sobre acesso SSH de qualquer endereço](../../assets/images/launch-ssh-warning.png)

Em **Configure storage**, utilize os valores de referência:

| Recurso | Configuração |
|---|---|
| Volume raiz | 8 GiB |
| Tipo de volume | gp3 |

![Configuração de armazenamento](../../assets/images/launch-storage.png)

### 5. Revise as opções avançadas

Se a seção **Advanced details** estiver disponível, revise as opções antes de iniciar

No ambiente de referência, **Credit specification** está definida como **Standard**

Essa configuração pode variar conforme o tipo de instância e as regras do laboratório

Mantenha as demais configurações autorizadas pela equipe

![Credit specification definida como Standard](../../assets/images/launch-credit.png)

### 6. Inicie a instância

Revise o painel **Summary**, verificando:

- Quantidade de instâncias: `1`
- AMI: Amazon Linux 2023
- Tipo: `t3.micro`
- Par de chaves selecionado
- Rede e armazenamento configurados

Se tudo estiver correto, clique em **Launch instance**

![Resumo da instância](../../assets/images/launch-summary.png)

Aguarde a mensagem de sucesso. Em seguida, use o caminho de navegação no topo da página e clique em **Instances** para abrir a lista de instâncias

![Confirmação de início da instância](../../assets/images/launch-success.png)

![Caminho no topo para abrir a lista de instâncias](../../assets/images/launch-instances-breadcrumb.png)

## Verificação

Na lista, selecione a instância criada e confira:

- **Instance state:** Running
- **Instance ID:** identificador da instância
- **Public IPv4:** endereço público, quando atribuído
- **Status checks:** verificações de funcionamento

![Instância selecionada na lista](../../assets/images/launch-instance-selected.png)

![Detalhes da instância com estado Running](../../assets/images/launch-instance-status.png)

<details>
<summary>Concluiu esta etapa? 🎉</summary>

<div align="center">

<img
  src="https://readme-typing-svg.demolab.com/?font=Fira+Code&amp;weight=600&amp;size=22&amp;duration=2500&amp;pause=1000&amp;color=FF9900&amp;center=true&amp;vCenter=true&amp;width=700&amp;height=75&amp;lines=Great+job%2C+Builder%21%3BEC2+instance+launched%21%3BReady+to+connect%3F"
  alt="EC2 instance launched"
/>

Seu servidor está pronto para a próxima etapa

</div>

</details>

---

<table width="100%">
  <tr>
    <td><a href="../console/README.md"><img src="https://img.shields.io/badge/Previous-374151?style=for-the-badge" alt="Previous"/></a></td>
    <td align="right"><a href="../connect/README.md"><img src="https://img.shields.io/badge/Next-374151?style=for-the-badge" alt="Next"/></a></td>
  </tr>
</table>
