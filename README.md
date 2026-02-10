# 🧔 Sistema de Agendamentos para Barbearia

<div align="center">

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

**Sistema completo de agendamento online para barbearias com painel administrativo**

[Demo](#) • [Recursos](#-recursos) • [Instalação](#-instalação) • [Uso](#-como-usar) • [Contribuir](#-contribuição)

</div>

---

## 📋 Sobre o Projeto

Sistema web moderno e responsivo para gerenciamento de agendamentos de barbearias. Desenvolvido com HTML, CSS e JavaScript puro, utilizando **localStorage** para persistência de dados, dispensando a necessidade de backend.

### ✨ Destaques

- 🎨 **Design Moderno** - Interface com glassmorphism e gradientes
- 📱 **100% Responsivo** - Funciona perfeitamente em mobile e desktop
- 💾 **Offline First** - Funciona sem conexão após primeiro carregamento
- 🚀 **Zero Dependências** - Apenas HTML, CSS e JavaScript puro
- ⚡ **Performance** - Leve e rápido

---

## 🎯 Recursos

### 👥 Para Clientes

- ✅ Cadastro e login de usuários
- ✅ Visualização de serviços disponíveis com preços
- ✅ Seleção de data e horário
- ✅ Visualização de horários disponíveis em tempo real
- ✅ Gerenciamento de agendamentos (visualizar e cancelar)
- ✅ Sistema de avaliação com estrelas e comentários
- ✅ Observações personalizadas para cada agendamento

### 👨‍💼 Para Administradores

#### 📊 Dashboard Completo
- Total de clientes cadastrados
- Agendamentos do dia
- Agendamentos pendentes
- Receita mensal

#### 📅 Gerenciamento de Agendamentos
- Visualizar todos os agendamentos
- Confirmar agendamentos pendentes
- Finalizar atendimentos com seleção de forma de pagamento:
  - 💵 Dinheiro
  - 📱 PIX
  - 💳 Débito
  - 💳 Crédito
- Cancelar agendamentos
- Solicitar avaliação do cliente

#### 👥 Gerenciamento de Clientes
- Lista completa de clientes
- Histórico de atendimentos
- Última visita de cada cliente

#### 💈 Gerenciamento de Serviços
- Adicionar novos serviços
- Definir duração e preço
- Remover serviços

#### ⭐ Sistema de Avaliações
- Visualizar todas as avaliações
- Média geral de avaliações
- Distribuição por estrelas
- Comentários dos clientes

#### ⚙️ Configurações Avançadas
- **Horários de Funcionamento**: Configure os horários disponíveis para agendamento
- **Dias de Ausência**: Bloqueie datas específicas (férias, feriados, etc.)
- **Informações Gerais**: Nome, telefone, email e endereço da barbearia

---

## 🛠️ Tecnologias Utilizadas

- **HTML5** - Estrutura semântica
- **CSS3** - Estilização moderna com:
  - Flexbox & Grid Layout
  - Glassmorphism
  - Animações e transições
  - Gradientes
- **JavaScript (ES6+)** - Lógica e interatividade
- **LocalStorage API** - Persistência de dados

---

## 📥 Instalação

### Opção 1: Download Direto

1. Faça o download do arquivo `barbearia-system.html`
2. Abra o arquivo em seu navegador
3. Pronto! O sistema está funcionando

### Opção 2: Clone do Repositório

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/sistema-barbearia.git

# Entre na pasta
cd sistema-barbearia

# Abra o arquivo HTML no navegador
# Windows
start barbearia-system.html

# macOS
open barbearia-system.html

# Linux
xdg-open barbearia-system.html
```

---

## 🚀 Como Usar

### Primeiro Acesso

O sistema vem com dados de demonstração pré-configurados:

**Credenciais de Administrador:**
- **Email:** admin@barbearia.com
- **Senha:** admin123

### Para Clientes

1. Acesse o sistema
2. Clique em "Cadastre-se"
3. Preencha seus dados
4. Faça login
5. Escolha um serviço
6. Selecione data e horário
7. Confirme o agendamento
8. Após o atendimento, avalie sua experiência

### Para Administradores

1. Faça login com as credenciais de admin
2. Acesse o painel de controle
3. Gerencie agendamentos, clientes e serviços
4. Configure horários e datas bloqueadas
5. Visualize estatísticas e avaliações

---

## ⚙️ Configuração

### Personalização

Todas as configurações podem ser ajustadas através do painel administrativo:

1. Faça login como administrador
2. Acesse a aba **"⚙️ Configurações"**
3. Configure:
   - Horários de funcionamento
   - Dias de ausência
   - Informações da barbearia

### Dados Padrão

O sistema inicializa com os seguintes serviços:

| Serviço | Duração | Preço |
|---------|---------|-------|
| Corte Simples | 30 min | R$ 35,00 |
| Corte + Barba | 45 min | R$ 55,00 |
| Barba | 25 min | R$ 25,00 |
| Corte Degradê | 40 min | R$ 45,00 |
| Hidratação Capilar | 60 min | R$ 70,00 |
| Sobrancelha | 15 min | R$ 15,00 |

---

## 📱 Capturas de Tela

### Tela de Login
Interface moderna com glassmorphism

### Dashboard do Cliente
Seleção de serviços e horários

### Painel Administrativo
Gestão completa de agendamentos

### Configurações
Personalização de horários e datas

---

## 🗂️ Estrutura do Projeto

```
sistema-barbearia/
│
├── barbearia-system.html    # Arquivo principal (HTML + CSS + JS)
├── README.md                 # Documentação
└── LICENSE                   # Licença MIT
```

---

## 💡 Funcionalidades Técnicas

### Gerenciamento de Estado

O sistema utiliza **localStorage** para persistência:

```javascript
DB = {
  users: [],           // Usuários cadastrados
  appointments: [],    // Agendamentos
  services: [],        // Serviços disponíveis
  ratings: [],         // Avaliações
  settings: {},        // Configurações
  blockedDates: [],    // Datas bloqueadas
  currentUser: null    // Usuário logado
}
```

### Segurança

- Autenticação básica com verificação de credenciais
- Separação de permissões (cliente/admin)
- Validação de dados antes de salvar

### Responsividade

- Mobile-first design
- Breakpoints otimizados
- Layout adaptável com Grid e Flexbox

---

## 🔄 Atualizações Futuras

- [ ] Notificações por email/SMS
- [ ] Integração com WhatsApp
- [ ] Exportação de relatórios em PDF
- [ ] Sistema de fidelidade
- [ ] Múltiplos barbeiros
- [ ] Pagamento online
- [ ] Backend com Node.js/PHP

---

## 🤝 Contribuição

Contribuições são sempre bem-vindas! Para contribuir:

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona MinhaFeature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um Pull Request

---

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 👨‍💻 Autor

**Felipe Andrade**

- LinkedIn: [Felipe Andrade]([https://linkedin.com/in/seu-perfil](https://www.linkedin.com/in/felipe-andrade-0331b9205/))
- Email: felipe.pessoall2026@gmail.com
- GitHub: [@felipeandrade08](https://github.com/felipeandrade08)

---

## 🙏 Agradecimentos

- Comunidade open source
- Todos que testaram e deram feedback
- Você por usar este sistema! ⭐

---

<div align="center">

### ⭐ Se este projeto foi útil, considere dar uma estrela!

**Desenvolvido com ❤️ por Felipe Andrade**

</div>
