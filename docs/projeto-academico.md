# Projeto acadêmico

**Título:** GCAM Portaria — gestão de portaria e controle de acesso para condomínios

**Autor:** Kauan Rafael Silva Sena

**Curso:** Análise e Desenvolvimento de Sistemas (ADS)

**Instituição:** FATEC Ribeirão Preto

## Contexto

A portaria precisa relacionar pessoas, unidades, autorizações e movimentações. Além do atendimento de visitantes, a rotina inclui correspondências, veículos, credenciais e equipamentos de acesso. Informações dispersas dificultam a conferência e a recuperação do histórico.

O projeto propõe integrar esses registros em uma aplicação para rede local, com separação entre as atividades do operador e as funções de administração.

## Objetivo geral

Desenvolver um sistema de gestão de portaria que reúna o cadastro de pessoas e veículos, o controle de visitas, o recebimento de correspondências e a comunicação com dispositivos de acesso.

## Objetivos específicos

- Relacionar condôminos e suas unidades, preservando os vínculos necessários à operação.
- Registrar autorizações, entradas, saídas e retiradas de correspondências.
- Controlar o acesso às funções por perfil e permissão.
- Integrar equipamentos sem acoplar os protocolos dos fabricantes às regras de negócio.
- Preservar as operações offline previstas e sincronizá-las após a reconexão.
- Verificar o comportamento do sistema com testes reproduzíveis.

## Método de desenvolvimento

O desenvolvimento ocorre de forma incremental. Cada fluxo envolve regras no servidor, persistência, interface e testes. Os componentes são separados por responsabilidade para permitir a evolução da operação da portaria e das integrações com dispositivos.

A avaliação combina testes unitários, testes de integração com banco isolado, testes de interface e verificações de instalação. A homologação dos equipamentos físicos é uma etapa própria; resultados simulados não são tratados como validação de campo.

## Delimitação

O escopo atual contempla servidor Windows, estações de portaria, operação em rede local e integrações específicas. O aplicativo macOS é utilizado como estação de testes. Um aplicativo móvel concluído, compatibilidade universal com fabricantes e certificação de segurança não fazem parte desta entrega.

Não são publicados resultados de implantação real sem evidências e autorização. A apresentação de um fluxo implementado não equivale à confirmação de seu uso em produção em um condomínio.

## Material de avaliação

Este repositório contém a apresentação técnica pública. Monografia, registros acadêmicos e eventual acesso da banca ao código são entregas distintas, a serem alinhadas com o orientador e com as regras do curso.

O repositório não publica código-fonte, credenciais, banco de dados ou cadastros reais. A disponibilização desta documentação não altera a licença do aplicativo.
