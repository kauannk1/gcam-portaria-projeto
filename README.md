<p align="center">
  <img src="assets/gcam-logo.png" alt="GCAM" width="112">
</p>

<h1 align="center">GCAM Portaria</h1>

<p align="center">Gestão de portaria e controle de acesso para condomínios.</p>

<p align="center">
  <a href="docs/projeto-academico.md">O TCC</a> ·
  <a href="docs/arquitetura.md">Arquitetura</a> ·
  <a href="docs/demonstracao.md">Demonstração</a> ·
  <a href="https://github.com/kauannk1/gcam-portaria-updates/releases/latest">Instaladores</a>
</p>

## Sobre o projeto

O GCAM Portaria foi desenvolvido para reunir, em um só sistema, os cadastros e as movimentações de uma portaria de condomínio. A proposta é facilitar a conferência de autorizações, preservar o histórico das operações e reduzir a dependência de registros separados dos equipamentos de acesso.

O projeto integra o Trabalho de Conclusão de Curso de **Análise e Desenvolvimento de Sistemas (ADS) da FATEC Ribeirão Preto**, desenvolvido por **Kauan Rafael Silva Sena**.

Este é o repositório de apresentação do projeto. Aqui estão o escopo, as decisões de arquitetura, o roteiro de demonstração e as informações de implantação. **O código-fonte permanece privado.**

## A rotina da portaria

O operador localiza o condômino responsável, registra o visitante e acompanha a entrada e a saída. A mesma aplicação permite receber correspondências, consultar veículos e conferir autorizações. As funções disponíveis dependem das permissões da conta utilizada.

| Área | O que o sistema permite |
| --- | --- |
| Condôminos | Organizar pessoas, unidades e vínculos de moradia |
| Visitas | Reaproveitar cadastros, registrar entradas e saídas e consultar o histórico |
| Pré-autorizações | Definir responsável, validade e horários de acesso |
| Correspondências | Registrar o recebimento e identificar quem realizou a retirada |
| Veículos e tags | Vincular veículos aos condôminos e administrar suas credenciais |
| Dispositivos | Configurar câmeras, terminais faciais, leitores e rotas |
| Administração | Gerenciar usuários, permissões, relatórios, auditoria e atualizações |

## Como funciona

Um computador mantém o servidor e o banco de dados. As estações de portaria se conectam a ele pela rede local. O servidor também realiza a comunicação com os equipamentos de controle de acesso.

Depois de um primeiro acesso conectado, a estação pode consultar informações já carregadas e registrar as operações previstas no modo offline. As pendências são enviadas automaticamente quando a conexão volta. A configuração de equipamentos, as funções administrativas e as liberações físicas pela estação dependem de conexão.

O reconhecimento facial é realizado pelo terminal. O GCAM gerencia o cadastro, a avaliação da fotografia, as autorizações e o envio das credenciais aos equipamentos compatíveis.

## Tecnologias

.NET 10 e ASP.NET Core no servidor, Avalonia na interface, PostgreSQL como banco de dados, Entity Framework Core na persistência e OpenCvSharp no processamento de imagens. As integrações com fabricantes são implementadas por adaptadores separados das regras de negócio.

## Situação atual

O sistema possui pacotes para Windows 10/11 x64 e uma estação de testes para macOS Apple Silicon. Há testes automatizados de regras de negócio, integração, interface e instalação.

O desenvolvimento e a validação continuam. A compatibilidade de um dispositivo depende do modelo, do firmware e da homologação em bancada. O primeiro terminal facial previsto para essa etapa é o **Hikvision DS-K1T671**. A existência de um adaptador não significa homologação de todos os equipamentos de uma marca.

O projeto não é apresentado como produto certificado, nem como solução imune a falhas. Antes da implantação, é necessário validar o ambiente, os equipamentos, os backups e os procedimentos da portaria. Veja os [critérios de implantação](docs/implantacao.md).

## Documentação

- [Contexto, objetivos e escopo acadêmico](docs/projeto-academico.md)
- [Arquitetura e decisões técnicas](docs/arquitetura.md)
- [Roteiro de demonstração](docs/demonstracao.md)
- [Implantação e uso em produção](docs/implantacao.md)
- [Etapas de validação](docs/validacao.md)
- [Uso do material e do software](AVISO-DE-USO.md)

## Distribuição e contato

Os instaladores e as atualizações ficam em um canal separado: [GCAM Portaria — distribuição](https://github.com/kauannk1/gcam-portaria-updates).

Para entrar em contato com o desenvolvedor, utilize o [perfil de Kauan no GitHub](https://github.com/kauannk1). Não publique dados de moradores, documentos, fotografias de pessoas, senhas ou cópias de bancos em comentários ou solicitações de suporte.

O nome da FATEC identifica o vínculo acadêmico do trabalho. Esta página não representa um canal institucional da faculdade nem uma declaração de aprovação ou certificação do produto.
