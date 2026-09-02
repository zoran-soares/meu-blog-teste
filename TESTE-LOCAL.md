# Teste local do Meu Blog Teste

## 1. Testar o site
No terminal, na pasta do projeto:

    npm run dev

Abra o endereço mostrado pelo `serve` (normalmente http://localhost:3000).

## 2. Testar somente a interface do painel, sem GitHub
Faça uma cópia de segurança de `admin/config.yml` e substitua temporariamente seu conteúdo pelo de `admin/config.local-test.yml`, renomeando o arquivo para `config.yml`.

Depois abra `/admin/` pelo servidor local.

O backend `test-repo` é próprio para testar o CMS, mas as alterações desaparecem ao recarregar a página.

## 3. Testar o CMS gravando no repositório local
Use a configuração `local_backend` descrita na documentação do Decap e execute `npx decap-server` na raiz do projeto. Isso é um teste mais avançado.

## 4. Antes do GitHub
Restaure `admin/config.yml` para a configuração de produção (`github`).

## 5. Git
    git add .
    git commit -m "Configura blog e painel Decap CMS"
    git push origin main
