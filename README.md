# resumo-nuvem-dio-3
Resumo do terceiro módulo de estudos sobre cloud.

Tipos de serviço de nuvem:

- IaaS (Infraestrutura como Serviço): Fornece recursos básicos como máquinas virtuais, redes e armazenamento. A gente gerencia o sistema operacional e as aplicações. Ideal quando precisamos de mais controle e flexibilidade, como em servidores personalizados.
- PaaS (Plataforma como Serviço): Fornece ambiente pronto para desenvolvimento, com ferramentas, runtime e banco de dados. Só focamos no código e nas aplicações. Bom para desenvolvedores que querem agilidade sem se preocupar com a infra.
- SaaS (Software como Serviço): Aplicações prontas acessadas pela internet, tipo o Outlook ou o Microsoft 365. Só usamos, sem precisar instalar ou manter nada. Ótimo para usuários finais.

Modelo de responsabilidade compartilhada:

Na nuvem, a responsabilidade pela segurança e gerenciamento é dividida entre o provedor (como a Microsoft) e o cliente. A divisão depende do tipo de serviço:

- IaaS: O provedor cuida da infra física, rede e virtualização. A gente cuida do sistema operacional, apps, dados e segurança.
- PaaS: O provedor já gerencia o sistema operacional e a plataforma. A gente cuida só das aplicações e dados.
- SaaS: O provedor cuida de tudo (infra, app, segurança). A gente só gerencia o uso e os dados.

# Dicas e atenções ao criar uma máquina virtual no Azure:

- Escolha o tamanho certo da VM: Nem sempre a maior é a melhor. Use o tamanho ideal para o que vai rodar, senão o custo fica alto sem necessidade.
- Selecione a região corretamente: Escolher uma região próxima dos usuários melhora o desempenho e pode até reduzir custos.
- Tipo de disco (HDD ou SSD): SSD é mais rápido, mas custa mais. Use SSD para apps que exigem performance e HDD para testes ou arquivos grandes.
- Sistema operacional: Veja se precisa de Windows ou Linux. Linux costuma ser mais barato por não ter licenças.
- Grupo de segurança de rede (NSG): Configure bem as portas abertas (tipo RDP ou SSH), só deixe o necessário para não correr riscos de segurança.
- Chave SSH ou senha forte: Se for Linux, prefira usar chave SSH. Se for Windows, use senha forte e segura.
- Tagueamento e nomes claros: Dê nomes e tags úteis pra identificar depois (como ambiente, projeto, dono). Ajuda na organização e controle de custos.
- Configurar backup e monitoramento: Ative backup se os dados forem importantes. E use o Monitor para acompanhar o desempenho da VM.
- Política de desligamento automático (opcional): Em ambientes de teste, dá pra configurar desligamento automático fora do horário útil e economizar grana.
