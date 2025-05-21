````markdown
# 📦 Boas Práticas com NPM

⚙️ Organização e controle de dependências são essenciais para manter o projeto leve, seguro e funcional.

---

## 🧹 Manutenção do Projeto

- ✨ **Mantenha o projeto limpo**: evite dependências desnecessárias.
- 📂 Se estiver usando `.gitignore`, rode:
  ```bash
  npm i
````

Isso carrega as dependências do `package-lock.json`.

* 🛠️ Para instalar pacotes de desenvolvimento:

  ```bash
  npm i log-symbols -D
  ```

  ✔️ Adiciona automaticamente aos `devDependencies`.

---

## 🔁 Correções e Ajustes

* ❌ Instalou um pacote errado?

  ```bash
  npm uninstall nome-do-pacote
  ```

  🧐 Confira o nome exato no `package.json` (em `dependencies` ou `devDependencies`).

* 🔍 Quer saber mais sobre os pacotes instalados?

  ```bash
  npm fund
  ```

  🔗 Lista as dependências e seus repositórios.

---

## ⬆️ Atualizações com Cuidado

* Para atualizar um pacote específico:

  ```bash
  npm update nome-do-pacote
  ```

⚠️ **Antes de atualizar:**

* Avalie se a nova versão pode causar **break changes**.
* Verifique se há riscos de **quebra no código em produção**.
* Leia sempre a documentação oficial.

🛡️ Atualize apenas se:

* Corrigir uma **vulnerabilidade crítica**.
* Melhorar a **segurança** da aplicação.

> 💥 *"Uma atualização brusca pode quebrar um código inteiro."*
> — **Felipão DIO**

---

## 🎨 Estilizando o Console com `chalk`

```js
import chalk from "chalk";

console.log(chalk.blue("Hello World"));
console.log(chalk.blue.bgBlackBright.bold("Outra funcionalidade da chalk."));
```

📌 Destaque visual para facilitar a leitura no terminal.

---

🚀 Mantenha a estrutura enxuta, segura e escalável.

