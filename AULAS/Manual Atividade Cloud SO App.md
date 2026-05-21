# Manual da Atividade — Cloud SO App 

## Introdução  
Foi desenvolvida uma aplicação web com **Node.js** e **Express.js** para exibir informações do sistema operacional usando o módulo `os`. O projeto foi executado localmente e publicado na nuvem (Render), permitindo comparar os dois ambientes.

## Objetivo  
Criar uma aplicação (`cloud-so-app`) que mostra dados como hostname, sistema operacional, CPU, memória e uptime, e comparar os resultados entre ambiente local e cloud.

## Tecnologias  
- Node.js  
- Express.js  
- HTML e CSS  
- Git e GitHub  
- Render  

## Funcionamento  
A aplicação cria um servidor web que, ao acessar `/`, exibe uma tabela com informações do sistema:

```js
os.hostname()
os.platform()
os.arch()
os.cpus()
os.totalmem()
os.freemem()
os.uptime()
```
---

## Execução

- Local: npm install → npm start → http://localhost:3000
- Cloud: deploy via Render conectado ao GitHub
- Resultado: https://cloud-app-so.onrender.com
- Local: dados da máquina do usuário (Windows, CPU física, memória real)
- Render: dados de um servidor em nuvem (geralmente Linux, recursos virtualizados)

---

## Conclusão

O projeto demonstrou que o mesmo código apresenta resultados diferentes dependendo do ambiente, reforçando conceitos de sistemas operacionais, virtualização e computação em nuvem.
