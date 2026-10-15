# Downloads e atualizações

O endereço oficial é:
https://github.com/kauannk1/gcam-portaria-projeto/releases/latest

## Escolher o arquivo

| Sistema | Arquivo |
| --- | --- |
| Windows 10/11 x64 | `GCAM-Setup-VERSAO.exe` |
| macOS Apple Silicon, estação de testes | `GCAM-Portaria-VERSAO-macOS-arm64.zip` |

O instalador Windows permite escolher servidor dedicado, servidor e portaria ou somente estação. Não é necessário baixar um instalador diferente para cada modo.

Os arquivos automáticos **Source code** do GitHub são cópias da documentação pública. Eles não instalam o programa e não contêm o código privado do GCAM.

## Atualizar uma instalação existente

O administrador pode utilizar **Configurações > Atualizações**. O aplicativo verifica o pacote antes de preparar a instalação. As versões atuais substituem o aplicativo e o reabrem; no Windows, a estação pode solicitar elevação administrativa.

A atualização do servidor é uma ação administrativa própria. Ela pode ser solicitada pela estação quando o servidor está disponível e possui os serviços gerenciados. O servidor baixa seu próprio instalador, preserva a instalação e prepara o banco quando há migrações pendentes. Atualizar somente o aplicativo Mac não substitui o servidor Windows.

## Transição do endereço antigo

As versões até 1.2.6 procuram o repositório `gcam-portaria-updates`. A versão 1.2.7 é publicada tanto nele quanto no projeto oficial. Depois de instalar essa versão, cliente e servidor passam a consultar o endereço oficial.

O endereço anterior permanece disponível com pacotes idênticos, sem depender de redirecionamentos de download. Não é necessário trocar o IP do servidor do condomínio, recriar a conta ou reinstalar o banco para mudar o canal de atualizações.

Se uma versão muito antiga não consegue buscar ou aplicar atualizações, faça essa primeira passagem pelo instalador atual. Não remova o banco nem desinstale o servidor apenas para trocar a versão.

## Cuidados

Mantenha um backup verificado antes de atualizar o servidor. Aguarde o envio das pendências offline e escolha uma janela de manutenção. A conferência de SHA-256 verifica a integridade do arquivo anunciado; ela não equivale a uma assinatura comercial do executável nem a uma auditoria de segurança.
