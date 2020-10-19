Title: Limites Operacionais
Description: Limites operacionais da plataforma 4biz.

# Limites Operacionais

Atualmente o 4biz opera adequadamente dentro dos seguintes limites de uso, considerando as configurações de hardware recomendadas descritas no documento de [Requisitos de Sistema](https://docs.run2biz.com/pt-br/4biz-helium/get-started/installation-and-upgrade/system-requirements.html#aplicacao-e-banco-de-dados-no-mesmo-servidor).

## Recomendações e limites para instalação on-premisses:

### Conexões de banco de dados:

- [x] Até 1200 conexões simultâneas entre o servidor de aplicação e o servidor de banco de dados.

### Tickets:

- [x] Abertura de até 200 tickets (incidentes ou requisições) por minuto.

### Analistas ou solicitantes interagindo com o 4biz através de sessões de navegador:

- [x] Até 100 sessões operando simultaneamente. 

### Sistemas automatizados que interagem via webservices ou outros métodos de integração (ex.: Telefonia, sistemas de monitoramento, sistemas legados, etc):

- [x] Até 50 sessões operando simultaneamente.

### Jobs:

- [x] Até 5 jobs sendo executados simultaneamente, desde que não utilizem, consumam ou acessem os mesmos recursos ou regras de negócio.


!!! note "NOTA"

    Recomendamos a instalação ou ampliação de ambiente clusterizado caso a sua operação ultrapasse os limites indicados acima.

!!! warning "ATENÇÃO"

    Importante observar que estes limites não são acumulativos. Ultrapassar qualquer um deles poderá causar degradação ou uma experiência inadequada do produto.  
    Qualquer dúvida favor consultar o suporte técnico.
