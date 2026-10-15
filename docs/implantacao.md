# Implantação e uso em produção

O GCAM Portaria é desenvolvido com a intenção de atender a operação de condomínios. Essa finalidade não dispensa a homologação do software, dos dispositivos e da infraestrutura de cada local.

## Formas de instalação

| Modo | Uso |
| --- | --- |
| Servidor e portaria | Um computador mantém os serviços e também a interface |
| Servidor dedicado | Um computador executa os serviços, sem depender da interface aberta |
| Estação | Um computador acessa o servidor pela rede |

Os serviços do servidor iniciam com o Windows. Os pacotes atuais atendem Windows 10/11 x64. O aplicativo macOS Apple Silicon é uma estação de testes conectada ao servidor, não uma instalação de servidor.

Os instaladores ficam no [canal de distribuição](https://github.com/kauannk1/gcam-portaria-updates/releases/latest). A disponibilidade do pacote não representa autorização de uso comercial ou certificação do ambiente. Os pacotes atuais não possuem certificado comercial de assinatura de código.

## Antes de colocar em operação

- Homologar os modelos e os firmwares dos dispositivos utilizados.
- Verificar comunicação, permissões e firewall, sem abrir o banco de dados à internet.
- Definir contas individuais e permissões compatíveis com a função de cada operador.
- Testar reinicialização do servidor e recuperação após queda de energia.
- Testar perda de rede, retomada e conferência das pendências.
- Verificar os procedimentos de entrada, saída e liberação local dos equipamentos.
- Manter backups protegidos e executar um teste de restauração em ambiente separado.
- Definir o procedimento da portaria para indisponibilidade e falha de equipamento.
- Avaliar a proteção, a finalidade e a retenção de dados pessoais e fotografias.
- Treinar os operadores e realizar uma implantação assistida antes da adoção definitiva.

## Atualizações

As atualizações são disponibilizadas em um canal separado da documentação. O aplicativo verifica os pacotes publicados; o administrador pode solicitar também a atualização do servidor pela estação.

O servidor é responsável pelas migrações do banco. Antes de uma atualização em ambiente real, mantenha backup verificado e planeje uma janela de manutenção. A confirmação de integridade do arquivo não substitui os testes de compatibilidade e funcionamento.

## Condições de uso

O aplicativo tem código-fonte privado. Os termos de licença, suporte e implantação devem ser definidos para cada distribuição ou contratação. A apresentação acadêmica não concede, por si só, uma licença comercial do programa.
