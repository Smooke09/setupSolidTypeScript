# Para utilizar

- Para utilizar esse repo e so clonar e ser fliz

# Documento para Aplicação

- Nessa aplicação utilizaremos as seguintes libs

# DevDependencies

- Express
- jest (Para teste unitários na aplicação)
- typescript-eslint/eslint-plugin (Para poder utilizar o eslint em conjunto com typescript)
- typescript-eslint/parser
- eslint (Para padronizar o código )
- eslint-config-prettier (Para poder utilizar o eslint junto com prettier e desativar regras do eslint que conflite com prettier)
- git-commit-msg-linter ( para poder padronizar as mensagem do commit no formato conventional commit)
- Husk (Para criar hooks de commit, definindo comando para ser executando antes do commit)
- lint-staged (Para executar comandos em arquivos que estão dentro do commit)
- prettier ( Para organiza)
- ts-jest (Para o Ts entender os test gerado pelo jest)
- ts-node ( Uma biblioteca que executa códigos typescript em tempo real)
- Nodemon ( server para nao precisar restarta a aplicação ele fica online o tempo todo)
- tsc-alias(Para compilar o relative path e converte ele para os paths normais que utilizamos )
- tsconfig-paths (Para poder usar os relatives paths com ts)
- typescript

# Padrões de commit

-- Nessa aplicação utilizaremos os padrões de commit convectional commit que consiste em 5 tipo de commit

- fix: Que seria correção em algo que estamos fazendo

- feat: Quando adicionamos alguma funcionalidade

- BREAKING CHANGE: Quando mudamos algo muito grande

- chore: quando fazemos alguma mudança relacionada a setup

# Scripts da Aplicação

- yarn start:dev (Server para iniciar o ambiente de desenvolvimento )

- husky:prepare (Criando arquivo de configuração do husky)

- test (Para se nao tiver nem um teste ele passar mesmo assim)

- test:watch( Teste que sera usado em ambiente dev)

- test:staged ( Script que sera executando com o lint-staged)

- build (Para bulida e compilar os arquivos TS )

- start ( Para iniciar o ambiente de produção)

- test:push ()

# Observações

- hooks pre-push nao esta funcionando na versão atual

- As vezes quando o pre commit buga podemos analisar caso nao ouve erro mesmo e confirmamos que foi bug podemos usar o 'npx prettier --write .' corrigir os problemas de formato de todos os arquivos não formatados

- Estamos utilizando relatives path onde podemos colocar @/ ao invés dos ../../

- As vezes voce pode clonar o repo e test e o husky nao funcionar ai voce so precisa refazer apagando a pasta husky e iniciando novamente com yarn:prepare e depois criar os pre-commit

- Para criar o primeiro pre-commit voce pode usar npx husky add .husky/pre-commit "yarn lint-staged"

- Para criar o pre-commit de conventional commit npx husky add .husky/commit-msg ".git/hooks/commit-msg $1" verifica se ficou uma aspa dentro do arquivo .husky pre-commit e remova
