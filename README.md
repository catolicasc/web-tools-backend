src/
├── adapters/
│   ├── express/         # Camada de apresentação utilizando o framework Express
│   ├── grpc/            # Camada de apresentação utilizando o protocolo gRPC
│   ├── message-broker/  # Camada de infraestrutura para gerenciar filas de mensagens
│   ├── mongodb/         # Camada de infraestrutura para acesso ao MongoDB
│   └── mysql/           # Camada de infraestrutura para acesso ao MySQL
├── domains/             # Camada de domínio do sistema, contendo as entidades, serviços e repositórios
│   ├── user/
│   │   ├── entity.js    # Entidade de usuário
│   │   ├── service.js   # Serviço de usuário
│   │   └── repository.js # Repositório de usuário
│   └── ...
├── usecases/            # Camada de aplicação do sistema, contendo as implementações dos casos de uso
│   ├── user/
│   │   ├── create-user.js # Caso de uso para criar um usuário
│   │   ├── update-user.js # Caso de uso para atualizar um usuário
│   │   └── list-users.js  # Caso de uso para listar todos os usuários
│   └── ...
├── shared/              # Camada compartilhada do sistema, contendo utilitários e ferramentas
│   ├── errors/          # Classes de erros customizadas
│   ├── middlewares/     # Middlewares para serem utilizados na camada de apresentação
│   ├── utils/           # Funções utilitárias para serem utilizadas em todo o sistema
│   └── ...
├── app.js               # Configuração da aplicação Express ou do servidor gRPC
├── server.js            # Código para inicializar o servidor HTTP ou gRPC
└── index.js             # Código principal para inicializar a aplicação
