🌉 Como operacionalizar a "Ponte" (Submodule)
Agora que você tem os arquivos no Hub, aqui está o comando exato que você rodará nos seus outros projetos (Spokes) para consumir essa inteligência sem duplicar código.

No terminal do seu projeto de pesquisa (ex: meu-projeto-acc):

Bash

# 1. Adiciona o Hub como uma pasta 'tools' (ou 'arsenal')
git submodule add https://github.com/aleeepassarelli/scientific-validation-hub.git tools

# 2. Linka a configuração de Pre-Commit do Hub para a raiz do seu projeto
ln -s tools/configs/pre-commit/.pre-commit-config.yaml .pre-commit-config.yaml

# 3. Instala os hooks (agora seu projeto está protegido pelo Hub)
pre-commit install
Vantagem Mágica: Quando você melhorar o .pre-commit-config.yaml lá no Hub central (por exemplo, adicionar flake8), basta ir nos seus projetos e rodar git submodule update --remote. Todos os seus projetos herdam a melhoria de segurança instantaneamente.
