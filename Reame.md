# ONG Pose da Liberdade 🌈

Repositório do site da ONG Pose da Liberdade, desenvolvido em **WordPress** com customizações em **HTML, CSS e JavaScript**.

---

## 📌 Tecnologias
- WordPress
- HTML5
- CSS3
- JavaScript

---

## 📂 Estrutura
```
/
├── wp-content/     # Temas e plugins customizados
├── wp-includes/    # Núcleo do WordPress
├── index.html      # Página inicial (caso exportado como estático)
└── ...
```

---

## 🚀 Como Rodar Localmente
1. Clone este repositório:
   ```bash
   git clone https://github.com/desyreegarcia/ong-pose.git
   ```
2. Configure um servidor local (XAMPP, WAMP ou similar).
3. Coloque os arquivos na pasta `htdocs` (ou equivalente).
4. Crie um banco de dados MySQL.
5. Configure `wp-config.php` com usuário, senha e nome do banco.
6. Acesse no navegador:  
   ```
   http://localhost/ong-pose
   ```

---

## 🌍 Deploy no GoogieHost

### 🔹 Opção 1 — WordPress Completo (com Banco de Dados)
1. **Criar conta no GoogieHost**  
   - Acesse [https://googiehost.com](https://googiehost.com) e crie uma conta gratuita.
   - Após criar a conta, acesse o **cPanel**.

2. **Adicionar o domínio**  
   - Caso tenha domínio próprio, adicione em **Domínios → Adicionar domínio**.  
   - Se não tiver domínio, use o subdomínio gratuito fornecido pelo GoogieHost.

3. **Enviar os arquivos**  
   - No **Gerenciador de Arquivos** ou via **FTP (FileZilla)**, acesse a pasta `public_html/`.
   - Faça upload de todos os arquivos do repositório (WordPress completo, incluindo `wp-content`, `wp-includes`, etc.).

4. **Configurar o banco de dados**  
   - No cPanel, crie um banco MySQL e um usuário.  
   - Dê permissão total ao usuário para o banco.  
   - Importe o dump do banco de dados (se existir).  

5. **Configurar o WordPress**  
   - Edite o arquivo `wp-config.php` com os dados do banco criado:
     ```php
     define('DB_NAME', 'nome_do_banco');
     define('DB_USER', 'usuario');
     define('DB_PASSWORD', 'senha');
     define('DB_HOST', 'localhost');
     ```
   - Salve e feche o arquivo.

6. **Acessar o site**  
   - Abra no navegador o domínio configurado (ou o subdomínio gratuito fornecido).  

---

### 🔹 Opção 2 — Site Estático (sem Banco de Dados)
Se você não quiser usar banco de dados, pode exportar o WordPress como **site estático**:

1. **Instalar o plugin [Simply Static](https://wordpress.org/plugins/simply-static/)** no WordPress local.  
2. **Gerar versão estática** (HTML + CSS + JS).  
3. Após a exportação, você terá uma pasta com apenas arquivos estáticos.  
4. Faça upload desses arquivos na pasta `public_html/` do GoogieHost.  
5. Acesse o domínio e o site funcionará sem banco de dados e sem necessidade de backend.  

> ✅ Essa opção é mais leve e ideal para hospedagem gratuita, já que não depende de PHP/MySQL.  
> 🚫 Porém, recursos dinâmicos (login, formulários de usuário, plugins que dependem de banco) não funcionarão.  

---

## 👥 Colaboradores
- [@desyreegarcia](https://github.com/desyreegarcia)  
- Equipe de desenvolvimento da ONG Pose da Liberdade

---

## 📄 Licença
Este projeto é de uso exclusivo da ONG Pose da Liberdade.
