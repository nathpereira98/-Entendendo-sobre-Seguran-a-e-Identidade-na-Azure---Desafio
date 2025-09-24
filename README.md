# -Entendendo-sobre-Seguran-a-e-Identidade-na-Azure---Desafio
 Desafio DIO - Entendendo sobre Segurança e Identidade na Azure

## Objetivo:
Compreender os conceitos, serviços e boas práticas relacionados à **identidade, autenticação e segurança** no Microsoft Azure, aplicando controles que melhorem a proteção de recursos e dados na nuvem.

## Entendimento: 
- **Microsoft Entra ID (Azure AD)**: gerenciamento de identidades, usuários, grupos e autenticação centralizada.  
- **Autenticação Multifator (MFA)**: fortalecer logins com fatores adicionais (algo que você sabe / possui / é).  
- **Acesso Condicional**: políticas que exigem condições (local, dispositivo, risco) antes de conceder acesso.  
- **RBAC (Role-Based Access Control)**: atribuição de permissões pelo princípio do menor privilégio.  
- **PIM (Privileged Identity Management)**: gerenciamento de acesso privilegiado just-in-time.  
- **Managed Identities**: identidades gerenciadas para recursos que acessam outros serviços sem credenciais embutidas.  
- **Modelo Zero Trust**: verificar sempre, conceder o mínimo necessário, segmentar e monitorar continuamente.  
- **Key Vault**: proteção e gerenciamento de segredos, chaves e certificados.  
- **Microsoft Defender para Nuvem**: detecção de ameaças, recomendações de segurança e postura de proteção para workloads.  
- **Azure Sentinel**: SIEM/SOAR para correlação de eventos, investigação e resposta a incidentes.  
- **Network Security**: NSGs, Azure Firewall e proteção DDoS para a camada de perímetro.  
- **Monitoramento e Logging**: habilitar logs de auditoria, diagnostic settings, Log Analytics e alertas para visibilidade e resposta.  
- **Governança e conformidade**: uso de Azure Policy e tags para padronizar e auditar recursos.

## Boas práticas (resumo rápido)
- Habilitar **MFA** para todas as contas com privilégios.  
- Aplicar **RBAC** em vez de papéis amplos (evitar *owner* desnecessário).  
- Usar **PIM** para elevação temporária de privilégios.  
- Adotar **Managed Identities** para aplicações e automações.  
- Armazenar segredos no **Key Vault**, nunca em código ou configurações abertas.  
- Definir **Access Policies** e **Conditional Access** para cenários de risco.  
- Centralizar logs e usar **Sentinel**/Log Analytics para detectar e responder.  
- Implementar **Azure Policy** para garantir conformidade (ex.: exigir criptografia).  
- Segmentar redes e aplicar **NSG/Firewall**; habilitar proteção DDoS.

## Exemplos práticos estudados
- Ativar MFA e configurar políticas de Acesso Condicional (ex.: exigir MFA em acessos externos).  
- Criar uma Managed Identity para um App Service e conceder acesso a um Key Vault.  
- Habilitar Diagnostic Logs para recursos e enviar para um workspace do Log Analytics.  
- Implementar uma política que exige tags e bloqueios (locks) para recursos críticos.

git branch -M main
git push -u origin main
