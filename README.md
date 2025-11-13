# Projeto - TrilhaTec

## Sumário
* [Descrição](#descrição)
* [Objetivo](#objetivo)

### Descrição

O **TrilhaTec** é uma caderneta digital desenvolvida em parceria com o **SENAC Paraná**, voltada especialmente aos estudantes do curso de Enfermagem. Seu principal objetivo é oferecer uma plataforma intuitiva para que os alunos registrem anotações durante as aulas e possam acessá-las durante os estágios. Conta com de Inteligência Artificial (IA) (simulação) para enriquecer o conteúdo e facilitar o aprendizado. Os instrutores, por sua vez, têm acesso às anotações dos alunos, incluindo aquelas enriquecidas com informações da IA. Isso permite um acompanhamento eficiente e uma análise criteriosa da qualidade do conteúdo, contribuindo para a formação de profissionais de saúde mais bem preparados.

### Objetivo

Criar uma solução digital para informatizar o processo de anotações acadêmicas, transportando as práticas tradicionais de registros em papel ou arquivos para uma aplicação funcional, fácil de usar e que integre recursos de inteligência artificial. 


### Tecnologias Utilizadas

- **HTML5**: Estruturação semântica das páginas e formulários da aplicação
- **CSS3**: Estilização avançada com suporte a modo claro/escuro, responsividade e animações
- **JavaScript ES6+**: Lógica de frontend, manipulação do DOM, gerenciamento de estado e integração com APIs
- **PHP 8.0+**: Backend para processamento de dados, autenticação e comunicação com banco de dados
- **MySQL 8.0+**: Sistema de gerenciamento de banco de dados relacional para armazenamento persistente
- **OpenAI API**: Integração com GPT-3.5/GPT-4 para análise e enriquecimento de conteúdo
- **LocalStorage**: Armazenamento local no navegador para preferências do usuário e cache temporário
- **GitHub**: Controle de versão e colaboração em equipe
- **VSCode**: Ambiente de desenvolvimento integrado


### Funcionalidades Principais

#### Sistema de Autenticação e Autorização

O sistema implementa um robusto mecanismo de login com três níveis de acesso distintos. A autenticação é realizada através de e-mail e senha, com validação tanto no frontend quanto no backend. As credenciais são verificadas contra o banco de dados MySQL, onde as senhas são armazenadas com hash seguro. O sistema mantém sessões ativas através de tokens seguros e oferece funcionalidade de logout que limpa todas as informações de sessão.

VÍDEO PARA DEMONSTRAÇÃO

**Credenciais de Acesso:**

- Aluno
- Instrutor
- Administrador

### Caderneta Digital Inteligente

A funcionalidade principal permite aos alunos criar, editar e organizar anotações de forma intuitiva. Cada anotação possui título, conteúdo detalhado, data de criação e modificação, além de categorias personalizáveis. O sistema oferece busca avançada por palavras-chave e organização cronológica automática. As anotações são sincronizadas em tempo real com o banco de dados, garantindo que não haja perda de informações.

VÍDEO PARA DEMONSTRAÇÃO

### Integração Avançada com Inteligência Artificial

O MedNotes integra-se com a API da OpenAI para oferecer análise automática e enriquecimento de conteúdo. Quando um aluno cria uma anotação, a IA analisa o contexto médico e de enfermagem, fornecendo sugestões complementares, esclarecimentos técnicos, referências bibliográficas relevantes e insights didáticos. O sistema também identifica possíveis inconsistências ou informações que necessitam de verificação adicional, alertando tanto alunos quanto professores.

VÍDEO PARA DEMONSTRAÇÃO

### Painel do Professor

Professores têm acesso a um dashboard completo onde podem visualizar todas as anotações de seus alunos, incluindo as sugestões geradas pela IA. O sistema oferece ferramentas de análise que permite fornecer feedback personalizado. Os professores podem também criar anotações compartilhadas e material de referência que ficam disponíveis para todos os alunos da turma.

VIDEO PARA DEMONSTRAÇÃO

### Sistema Administrativo

Administradores possuem controle total sobre o sistema, incluindo gerenciamento completo de usuários com capacidade de criar, editar e excluir contas, estatísticas de uso e engajamento, configuração de parâmetros da IA e suas integrações, backup e recuperação de dados, e monitoramento de performance do sistema.

VIDEO PARA DEMONSTRAÇÃO

### Interface Adaptável com Modo Claro/Escuro

O sistema implementa alternância completa entre modo claro e escuro, mantendo consistência visual e usabilidade em ambos os temas. A preferência do usuário é salva automaticamente no localStorage, garantindo que a escolha seja lembrada em sessões futuras. O modo escuro foi especialmente otimizado para reduzir fadiga ocular durante uso prolongado, melhorando a acessibilidade para usuários com sensibilidade à luz ou necessidades específicas de visualização.

VIDEO PARA DEMONSTRAÇÃO

### Sistema de Notificações e Lembretes

Implementação de notificações inteligentes que alertam alunos sobre atualizações importantes, sugestões da IA que requerem atenção, feedbacks de professores e lembretes para revisão de conteúdo.

### Backup e Sincronização

Sistema automatizado de backup que garante que todas as anotações sejam preservadas e possam ser recuperadas em caso de problemas técnicos. Sincronização em tempo real entre diferentes dispositivos, permitindo que alunos acessem suas anotações de qualquer lugar. Exportação de anotações em diversos formatos (PDF, Word, texto simples) para uso offline ou impressão.


### Para Estudantes de Enfermagem

Durante as aulas teóricas, os alunos podem registrar rapidamente conceitos importantes, procedimentos clínicos e observações do professor. A IA automaticamente enriquece essas anotações com informações complementares sobre anatomia, farmacologia ou protocolos de cuidado. Durante estágios práticos, os alunos acessam suas anotações organizadas por tema, com sugestões da IA sobre melhores práticas e cuidados específicos para cada situação clínica encontrada.

### Para Professores e Orientadores

Professores podem acompanhar o progresso de aprendizagem de cada aluno através das anotações registradas, identificando lacunas de conhecimento ou conceitos mal compreendidos. O sistema permite fornecer feedback direcionado e personalizado, além de criar material de apoio baseado nas dúvidas mais comuns identificadas nas anotações dos alunos.

### Para Administradores Acadêmicos

Gestores educacionais podem analisar dados agregados sobre efetividade do ensino, identificar disciplinas ou tópicos que apresentam maior dificuldade para os alunos, e otimizar curriculos baseados em dados reais de aprendizagem. O sistema também oferece métricas sobre engajamento dos alunos e efetividade dos recursos de IA implementados.


## Arquitetura do Sistema

### Frontend
Interface responsiva desenvolvida com HTML5 semântico, CSS3 moderno com variáveis customizáveis para temas, e JavaScript modular com padrões de desenvolvimento limpo.

### Backend
API RESTful desenvolvida em PHP com arquitetura MVC, implementando padrões de segurança como validação de entrada, sanitização de dados e prevenção contra ataques comuns (SQL Injection, XSS, CSRF). Sistema de roteamento limpo e middleware para autenticação e autorização.

### Banco de Dados
Esquema relacional otimizado com tabelas para usuários, anotações, sessões e configurações. Implementação de índices apropriados para performance em consultas complexas e backup automatizado com retenção configurável.

### Integração Externa

Comunicação segura com API da OpenAI através de endpoints protegidos. Sistema de fallback para casos de indisponibilidade da API externa. Este estágio foi simulado no projeto que conta com respostas da própria IA, no entanto, sem a integração direta, uma vez que há um custo para as consultas feitas na aplicação.


### 📱 Responsividade e Acessibilidade

O TrilhaTec foi desenvolvido seguindo princípios de design responsivo, garantindo experiência otimizada em dispositivos móveis, tablets e desktops. A interface adapta-se automaticamente a diferentes tamanhos de tela, mantendo usabilidade e funcionalidade completas. Além disso conta com recurso de modo escuro, uma vez que este pode ser considerado um recurso de acessibilidade. 


## Roadmap e Futuras Implementações

* **Fase 1 - Melhorias Visuais e UX** - Redesign completo da interface com foco em experiência do usuário, implementação de animações e micro-interações, otimização para dispositivos móveis, e personalização avançada de temas e layouts.
* **Fase 2 - Integrações Avançadas** - Integração com sistemas acadêmicos existentes, API para aplicativos móveis nativos, conectividade com dispositivos wearables para coleta de dados em tempo real durante estágios, e integração com bibliotecas médicas digitais.
* **Fase 3 - Inteligência Artificial Avançada** - Implementação de modelos de IA especializados em conteúdo médico, sistema de recomendação personalizado baseado em padrões de aprendizagem, análise preditiva para identificação precoce de dificuldades de aprendizagem, e geração automática de questionários e exercícios baseados nas anotações.
* **Fase 4 - Recursos Colaborativos Expandidos** - Salas virtuais para estudo em grupo, sistema de mentoria peer-to-peer, gamificação com conquistas e progressão, e marketplace de conteúdo onde professores podem compartilhar material premium.


### Responsáveis pelo desenvolvimento do projeto

* Orientador - [Leonardo Rocha](https://github.com/leonardossrocha)  

* Alunos:  
[Heitor Dalla](https://github.com/HeitorDalla)
[Gilherme Tofoli](https://github.com/guilhermetofoli)
[Matheus Coronado](https://github.com/matheuscoronado)  
[Abner Castanho](https://github.com/abnercastanho)  
[Gabriel Coronado](https://github.com/BackupTrabalho1212)  