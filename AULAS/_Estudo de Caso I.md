
## Estudo de Caso I – RELATÓRIO DE PLANEJAMENTO DE INFRAESTRUTURA 

---

## 1. Introdução

A DevStore é uma startup de desenvolvimento web que enfrenta dificuldades relacionadas à organização, escalabilidade e segurança de sua infraestrutura de TI. Atualmente, utiliza servidores locais sem padronização e desenvolve aplicações diretamente nas máquinas dos programadores, sem separação entre ambientes.

Esse cenário aumenta o risco de falhas, dificulta a manutenção e compromete a qualidade dos sistemas. Assim, este relatório propõe uma solução baseada em virtualização, containerização e computação em nuvem.

---

## 2. Problemas Identificados

Os principais problemas incluem a falta de padronização dos servidores, limitação de escalabilidade devido ao uso exclusivo de infraestrutura local e ausência de ambientes separados para desenvolvimento, testes e produção.

Além disso, não há uso de testes automatizados nem integração contínua, o que aumenta a chance de erros. Também existem falhas na segurança, como ausência de controle de acesso e monitoramento adequado.

---

## 3. Objetivos da Solução

A proposta busca organizar a infraestrutura, garantir ambientes padronizados e permitir escalabilidade conforme a demanda. Também visa melhorar a segurança e reduzir custos operacionais, utilizando soluções mais modernas e eficientes.

---

## 4. Arquitetura Proposta

A solução integra virtualização, containerização, nuvem e segurança.

Máquinas virtuais serão usadas principalmente para testes, oferecendo isolamento. Já os containers, com uso de Docker, serão a base para execução das aplicações, garantindo leveza e consistência.

A produção será hospedada na nuvem (AWS ou Azure), permitindo alta disponibilidade e escalabilidade. Também serão implementadas medidas de segurança como controle de acesso, firewall e monitoramento contínuo.

---

## 5. Descrição da Arquitetura

A estrutura é dividida em três camadas: desenvolvimento, testes e produção.

No desenvolvimento, os programadores utilizam containers para padronizar o ambiente. Nos testes, são usados containers e máquinas virtuais para validação das aplicações. Já na produção, os sistemas são executados na nuvem com foco em desempenho e disponibilidade.

Uma camada de controle central gerencia acesso, automação e monitoramento.

---

## 6. Papel dos Sistemas Operacionais

Os sistemas operacionais gerenciam recursos e executam aplicações em todas as etapas.

Nos containers, o kernel é compartilhado, tornando-os mais leves. Já nas máquinas virtuais, cada ambiente possui seu próprio sistema operacional. Na nuvem, sistemas Linux são geralmente utilizados por sua estabilidade e desempenho.

---

## 7. Fluxo de Trabalho

O processo inicia no desenvolvimento com containers, segue para testes em ambientes isolados e, após validação, é implantado na nuvem. Depois disso, os sistemas são monitorados continuamente.

---

## 8. Monitoramento e Infraestrutura

O monitoramento permite acompanhar desempenho e identificar falhas. A infraestrutura inclui redes virtuais seguras e armazenamento escalável, garantindo proteção e flexibilidade.

---

## 9. Justificativa

A adoção dessas tecnologias melhora o desempenho, reduz custos e facilita a manutenção. Containers e nuvem tornam o sistema mais flexível e preparado para crescer.

---

## 10. Implantação e Manutenção

A implementação será gradual, com migração para a nuvem e adoção de containers. A manutenção incluirá monitoramento contínuo, atualizações e backups regulares.

---

## 11. Conclusão

A solução proposta torna a infraestrutura mais moderna, segura e escalável, atendendo às necessidades da DevStore e permitindo seu crescimento sustentável.

---

## 12. Comparação de Custos

### Infraestrutura Local  
Exige alto investimento inicial em hardware, além de custos contínuos com energia, manutenção e equipe.

👉 **Custo estimado:** R$ 800 a R$ 2.000/mês (sem contar investimento inicial)

---

### Computação em Nuvem  
Funciona sob demanda, com pagamento conforme o uso.

👉 **Custo estimado:** R$ 300 a R$ 1.500/mês

---

### Análise Final

A nuvem oferece maior flexibilidade, escalabilidade e menor custo inicial, sendo mais adequada para startups. Já a infraestrutura local exige mais investimento e manutenção.

---

### Conclusão dos Custos

Para a DevStore, a computação em nuvem é a melhor escolha, pois reduz custos iniciais, facilita a expansão e melhora a eficiência operacional.
