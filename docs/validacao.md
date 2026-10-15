# Validação e próximos passos

## Tipos de verificação

| Verificação | O que procura demonstrar |
| --- | --- |
| Testes unitários | Comportamento das regras e dos componentes isolados |
| Testes de integração | Comunicação da API com persistência e fluxos do servidor |
| Testes de interface | Comportamento dos controles e seu ciclo de vida |
| Testes de instalação | Preparação dos serviços, autenticação, reinstalação e preservação dos registros |
| Homologação física | Compatibilidade e comportamento no modelo e firmware do equipamento |
| Implantação assistida | Adequação da solução à rotina e à infraestrutura do local |

Uma verificação não substitui a outra. Testes automatizados aprovados não comprovam compatibilidade universal, ausência de vulnerabilidades ou disponibilidade contínua em produção.

## Referência de desenvolvimento

Na revisão 1.2.6 foram executados 144 testes unitários e seis testes de interface. Os testes de interface foram executados também em ambientes Windows e macOS no GitHub Actions. As verificações de instalação são mantidas separadamente no repositório privado de desenvolvimento.

Esses números se referem a uma revisão específica. Não são apresentados como resultado de uma auditoria independente ou de um estudo de campo.

## Próximas etapas

1. Homologar o terminal Hikvision DS-K1T671 em bancada, identificando o firmware utilizado.
2. Conferir envio de credenciais, retorno de eventos, entrada, saída e comportamento sem rede.
3. Validar os leitores de tags nos modelos efetivamente utilizados.
4. Revisar os procedimentos de backup, restauração e atualização em um ambiente semelhante ao de implantação.
5. Realizar a avaliação de uso com operadores, sem dados pessoais reais na apresentação pública.
6. Registrar os resultados e incorporar os ajustes encontrados antes da implantação definitiva.

Não há, neste repositório, declaração de homologação concluída ou de implantação real sem evidências que a sustentem.
