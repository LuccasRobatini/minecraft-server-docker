# Minecraft Server com Docker

Servidor Minecraft privado com suporte a crossplay Java e Bedrock, rodando em containers Docker no CanelSystem Homelab.

---

##  Objetivo

Hospedar um servidor para amigos com configuração simplificada via Docker, suporte a múltiplos clientes e plugins administrativos — enquanto pratico administração Linux, Docker e troubleshooting de rede.

---

##  Stack

- **Base:** Purpur (fork de Paper)
- **Crossplay:** Geyser-Spigot + Floodgate
- **Containers:** Docker
- **Acesso externo:** playit.gg
- **OS:** Ubuntu Server 24.04 LTS

---

##  Plugins

| Plugin | Função |
|---|---|
| Geyser-Spigot | Crossplay Java/Bedrock |
| Floodgate | Autenticação para jogadores Bedrock |
| EssentialsX | Comandos utilitários |
| LuckPerms | Sistema de permissões |
| CoreProtect | Logs e proteção de blocos |
| ViaVersion | Compatibilidade entre versões |
| Simple Voice Chat | Chat de voz para Java |
| SimpleVoice-Geyser | Suporte ao voice chat no Bedrock |

---

##  Rede

- Acesso externo via **playit.gg** (sem necessidade de IP público fixo)
- Portas TCP e UDP configuradas para Java, Bedrock e Voice Chat
- IP local do servidor fixo via reserva DHCP

> Tentativa de uso do Cloudflare Tunnel para Simple Voice Chat no Bedrock não foi viabilizada — o serviço requer porta 80 aberta de forma contínua, o que não era compatível com o ambiente.

---

## ⚠️ Aviso

Tokens, senhas e configurações sensíveis não estão publicados neste repositório.
