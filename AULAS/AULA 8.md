##  Dashboard-Stats-SO - Projeto de Sistemas Operacionais

## Objetivo da Aplicação

Exibir dados reais do ambiente onde a aplicação está executando: máquina local ou Render/cloud, de forma simples e eficiente.

## Links do projeto

**Teste online da Aplicação no Render:**  
https://your-react-canvas-2.onrender.com/

---

## Tecnologias

- Node.js
- Express
- CORS
- Módulos nativos: `os`, `fs`, `path`, `process`
- HTML, CSS e JavaScript puro

---

## Instalação

```bash
npm install
```

---

## Execução local

```bash
npm start
```

Acesse:

```text
http://localhost:3000
```

---

## Deploy no Render

Configuração sugerida:

- **Build Command:** `npm install`
- **Start Command:** `npm start`
- **Environment:** Node
- **Port:** definida automaticamente via `process.env.PORT`

A aplicação funciona localmente e no Render sem URL local hardcoded.

---

## Rotas disponíveis

- `GET /` — Dashboard visual completo
- `GET /api/system` — Informações do sistema em JSON
- `GET /health` — Health check simples em JSON

---

## Informações exibidas

### Resumo executivo

- Uso de RAM
- Uso médio aproximado de CPU
- Uptime
- Quantidade de arquivos
- IP principal
- Status da máquina

### Sistema

- Hostname
- Tipo do SO
- Release/kernel
- Plataforma
- Arquitetura
- Endianness
- Versão do Node.js

### Usuário/processo

- Usuário atual
- Diretório home
- Diretório temporário
- Shell
- UID e GID quando disponíveis

### RAM

- Memória total
- Memória usada
- Memória livre
- Memória do processo Node.js
- Barra visual de consumo

### CPU

- Núcleos
- Modelo
- Load average
- Uso aproximado por núcleo
- Barras visuais

### Rede

- IP principal
- Interfaces de rede
- Endereços IPv4/IPv6
- Tipo interno/externo

### Arquivos

- Lista de arquivos relevantes
- Tipo
- Tamanho

### Tempo

- Uptime formatado
- Timezone UTC
- Timestamp ISO

### Aplicação

- PID
- Diretório atual
- Caminho do executável Node.js
- Memória do processo

### Ambiente

- Local ou Render/cloud
- `PORT`
- `NODE_ENV`
- Indício de cloud/AWS
- Mensagem de status

---

## Conceitos de Sistemas Operacionais demonstrados

- Gerenciamento de memória
- Monitoramento de CPU
- Processos e PID
- Usuários do sistema
- Sistema de arquivos
- Interfaces de rede
- Uptime e tempo do sistema
- Diferenças entre execução local e em nuvem

---

## Simulação avançada de SO

O dashboard inclui uma simulação simples no navegador para demonstrar:

- Alocação de memória
- Liberação de memória
- Criação de processo simulado
- Encerramento de processo simulado
- Fila de processos
- Blocos de memória livres e ocupados

A simulação é frontend-only para manter o projeto simples, estável e fácil de explicar em apresentações.

---

## Comparação: execução local vs Render/cloud

### Execução local

Os dados refletem o computador do desenvolvedor:

- Hostname
- Usuário
- Diretórios
- Memória
- Interfaces de rede da máquina local

### Execução no Render/cloud

Os dados refletem o container/servidor disponibilizado pela plataforma.

Alguns campos podem ser diferentes ou limitados por segurança, como:

- Shell
- UID/GID
- Hostname temporário
- IP interno
- Variáveis de ambiente

---

## Comparação: Render vs Railway

### Render

- Deploy simples para projetos acadêmicos
- Detecta automaticamente `process.env.PORT`
- Integração fácil com Git

### Railway

- Estrutura organizada por ambientes e serviços
- Mais voltado para aplicações compostas por múltiplos serviços
- Deploy igualmente compatível com Node.js

Ambas as plataformas suportam:

- Build command
- Start command
- Deploy de aplicações Node.js

---

## Conclusão

O projeto demonstra como uma aplicação Node.js pode consultar informações do Sistema Operacional usando módulos nativos e apresentar esses dados em um dashboard web.

A mesma base funciona localmente e na nuvem, permitindo:

- Comparação entre ambientes
- Observação de diferenças de infraestrutura
- Relação prática com conceitos de Sistemas Operacionais
