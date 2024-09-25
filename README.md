# Laboratório de Segurança e Identidade na Azure

Este repositório documenta um laboratório prático focado em Segurança e Identidade na Azure. Exploramos práticas recomendadas para proteger recursos e gerenciar identidades de forma segura utilizando ferramentas e serviços nativos da plataforma.

## Sumário

1. [Visão Geral](#visão-geral)
2. [Serviços Utilizados](#serviços-utilizados)
3. [Políticas de Acesso Condicional](#políticas-de-acesso-condicional)
4. [Controle de Acesso Baseado em Função (RBAC)](#controle-de-acesso-baseado-em-função-rbac)
5. [Autenticação Multifator (MFA)](#autenticação-multifator-mfa)
6. [Monitoramento e Conformidade](#monitoramento-e-conformidade)

---

## Visão Geral

Neste laboratório, foram aplicados conceitos de segurança para proteger identidades e controlar o acesso aos recursos da Azure, utilizando serviços como **Azure Active Directory (Azure AD)**, **Políticas de Acesso Condicional** e **Autenticação Multifator (MFA)**.

A segurança de identidades e a proteção de recursos são fundamentais em um ambiente de nuvem. Este laboratório implementa uma abordagem de **Zero Trust**, onde o acesso é continuamente monitorado e a segurança é aplicada em múltiplas camadas.

## Serviços Utilizados

- **Azure entra ID**: Serviço de gerenciamento de identidades e controle de acesso.
- **Defender for Cloud**: Ferramenta para monitoramento contínuo de segurança e gerenciamento de postura de segurança (CSPM).
- **RBAC (Role-Based Access Control)**: Modelo de controle de acesso com permissões baseadas em funções.
- **Políticas de Acesso Condicional**: Gerenciamento de acesso baseado em condições dinâmicas.
- **Autenticação Multifator (MFA)**: Proteção adicional para a verificação de identidade.

## Políticas de Acesso Condicional

As **Políticas de Acesso Condicional** foram configuradas para garantir que somente usuários verificados possam acessar recursos. A política implementada inclui:

- **Condição de Localização**: Bloquear logins a partir de locais não confiáveis.
- **Verificação do Dispositivo**: Permitir acesso apenas de dispositivos gerenciados ou com conformidade verificada.
- **Autenticação Multifator**: Requerer MFA para tentativas de login de fora do ambiente corporativo.

## Controle de Acesso Baseado em Função (RBAC)

Utilizamos **RBAC** para garantir que os usuários tenham o nível mínimo de acesso necessário:

- **Owner**: Controle total sobre o recurso, incluindo delegação de acesso.
- **Contributor**: Pode gerenciar recursos, mas sem delegação de permissões.
- **Reader**: Somente leitura dos recursos.
  
RBAC foi aplicado a diferentes escopos, desde **grupos de recursos** até **recursos individuais**, reforçando o princípio do **menor privilégio**.

## Autenticação Multifator (MFA)

A **Autenticação Multifator (MFA)** foi implementada como uma camada adicional de segurança, exigindo uma segunda forma de verificação (como uma mensagem no celular ou aplicativo de autenticação) além da senha.

Isso adiciona uma barreira contra comprometimento de credenciais e garante que o acesso só seja concedido após uma verificação robusta.

## Monitoramento e Conformidade

O **Defender for Cloud** foi usado para monitorar continuamente a postura de segurança e fornecer recomendações de conformidade. Este serviço ajuda a manter a segurança do ambiente de nuvem em conformidade com normas como **ISO 27001** e **NIST**.

- **Pontuação de Segurança**: A ferramenta sugere melhorias e aumenta a **Secure Score**, indicando o nível de segurança do ambiente.
---

Este laboratório fortalece a compreensão da segurança na nuvem e gestão de identidades na Azure, aplicando práticas recomendadas de Zero Trust e monitoramento contínuo para uma postura de segurança eficaz.
