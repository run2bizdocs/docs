Title: Ativar o Builder

# Ativar o Builder

Para a integração 4biz/Builder funcionar, você deve:

- Ter a versão 8.0.0.0 ou superior da 4biz
- Ter o 4biz configurado para acesso HTTPS: //
- Ter os parâmetros de integração configurados no 4biz


![Builder Conection][1]

- **Parâmetro 309:**

    ```sh
    Value: Yes
    ```

- **Parâmetro 310:**

Exemplo:

    ```sh
    https://localhost:8443/cit-esi-web
    ```

- **Parâmetro 311:**

Exemplo:

    ```sh
    4biz.local\builder.user
    ```
    

!!! success "USUÁRIO Builder"
    Para que a integração funcione corretamente é necessário que o usuário de serviço criado para o Builder contenha no campo login o atributo de identificação do domínio, ou seja, "4biz.local" (ex. O usuário "Builder" deverá ter no campo login a seguinte informação  "4biz.local\builder.user").


[1]:images/builder-conection.png
