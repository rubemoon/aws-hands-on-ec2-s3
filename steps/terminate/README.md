
<p align="center">
  <a href="../../README.md"><img src="../../assets/images/step-header.png" alt="AWS Student Builder Group at UFFS Chapecó — voltar ao laboratório" width="100%" /></a>
</p>

<div align="center">

<h2>05 · Encerrando uma instância EC2</h2>

<a href="../console/README.md"><img src="https://img.shields.io/badge/01-Console_AWS-374151?style=for-the-badge" alt="Console AWS"/></a>
<a href="../launch/README.md"><img src="https://img.shields.io/badge/02-Criar_EC2-374151?style=for-the-badge" alt="Criar EC2"/></a>
<a href="../connect/README.md"><img src="https://img.shields.io/badge/03-Conectar_EC2-374151?style=for-the-badge" alt="Conectar EC2"/></a>
<a href="../metadata/README.md"><img src="https://img.shields.io/badge/04-Metadados-374151?style=for-the-badge" alt="Metadados"/></a>
<img src="https://img.shields.io/badge/05-Encerrar-FF9900?style=for-the-badge" alt="Etapa atual"/>

</div>

## Visão geral

Ao finalizar um laboratório na AWS, é importante encerrar os recursos que não serão mais utilizados

Nesta etapa, vamos terminar a instância EC2 criada para o laboratório e confirmar que ela chegou ao estado `Terminated`

> **Atenção:** terminar uma instância é uma ação permanente e não pode ser desfeita. Os dados do volume raiz EBS podem ser excluídos conforme a opção **Delete on termination**; confira as configurações de armazenamento antes de continuar. Outros volumes EBS podem permanecer e continuar gerando custos

## Instruções

### 1. Localize sua instância

No AWS Console, abra **EC2 → Instances** e selecione a instância deste laboratório

Confira o nome ou outro identificador da instância selecionada antes de prosseguir. Não termine outras instâncias da conta

### 2. Solicite o encerramento

Com a instância correta selecionada, abra o menu **Instance state**

![Menu Instance state com a opção Terminate (delete) instance](../../assets/images/terminate-instance-state.png)

Escolha **Terminate (delete) instance**. Não escolha **Stop instance** se o objetivo for encerrar permanentemente o recurso

### 3. Confirme a operação

Leia o aviso e confirme que selecionou a instância correta e que não precisa dos dados que serão excluídos

![Aviso do Console sobre a exclusão do volume raiz EBS](../../assets/images/terminate-ebs-warning.png)

Se tiver certeza, clique em **Terminate (delete)**

![Botão para confirmar Terminate (delete)](../../assets/images/terminate-confirm-button.png)

### 4. Verifique o estado

Aguarde o Console atualizar o estado. Ele pode passar por:

`Running → Shutting-down → Terminated`

## Verificação

Na lista **Instances**, confirme que **Instance state** da instância selecionada apresenta `Terminated`. A atualização pode levar alguns instantes

Depois, confira **Volumes** e outros recursos relacionados para garantir que não restaram recursos que você não pretende manter

<details>
<summary>Qual a diferença entre Stop e Terminate?</summary>

- **Stop:** desliga a instância, permitindo iniciá-la novamente. Os volumes EBS continuam existindo e podem gerar custos
- **Terminate:** encerra permanentemente a instância. O volume raiz EBS é excluído se **Delete on termination** estiver habilitado; outros volumes EBS podem permanecer

</details>

<details>
<summary>Laboratório concluído! 🎉</summary>

<div align="center">

<img
  src="https://readme-typing-svg.demolab.com?font=Fira+Code&amp;weight=600&amp;size=22&amp;duration=2500&amp;pause=1000&amp;color=FF9900&amp;center=true&amp;vCenter=true&amp;width=700&amp;height=75&amp;lines=Congratulations%2C+Builder!;EC2+Lab+Completed!;Keep+Building%21"
  alt="EC2 Lab Completed"
/>

### Parabéns, Builder!

Você concluiu seu primeiro laboratório Amazon EC2

Criou uma instância, conectou-se ao servidor Linux, explorou seus metadados e encerrou os recursos utilizados

**[Voltar ao laboratório](../../README.md)**

</div>

</details>

---

<table width="100%">
  <tr>
    <td><a href="../metadata/README.md"><img src="https://img.shields.io/badge/Previous-374151?style=for-the-badge" alt="Previous"/></a></td>
    <td align="right"></td>
  </tr>
</table>
