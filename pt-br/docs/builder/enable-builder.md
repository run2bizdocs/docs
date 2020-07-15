Title: Ativar o Builder

# Ativar o Builder

Os requisitos para ativar o Builder no 4Biz são:

- Ter a versão Helium ou superior do 4biz
- Ter o 4biz configurado para acesso HTTPS
- Configurar os seguintes parâmetros de integração:

--


- Parâmetro 309:

    ```
    Value: Yes
    ```

- Parâmetro 310:

    ```
    https://localhost:8443/cit-esi-web
    ```
	
Note que se o Builder não residir na mesma máquina que o 4Biz, localhost deverá ser alterado para o nome do servidor no qual o Builder está 
instalado.

- Parameter 311:

    ```
	dominio\usuario
	```

	
Para que a integração funcione corretamente é necessário que a configuração do nome do usuário Builder contenha a identificação do domínio do qual ele faz parte. Por exemplo: 4biz.local\builder.
