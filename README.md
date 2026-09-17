# Yago Barbershop 💈

Sistema de agendamento e gerenciamento desenvolvido para uma barbearia.

A aplicação permite que clientes façam agendamentos online e que o barbeiro acompanhe e gerencie sua agenda através de uma área administrativa.

**Aplicação:** https://saasbarber.onrender.com/

**Tecnologias:** Next.js · TypeScript · React · Supabase · PostgreSQL

---

## Sobre o projeto

O projeto foi criado para substituir parte do controle manual de agendamentos feito através do WhatsApp.

A ideia era ter um sistema simples para o cliente agendar um horário e, ao mesmo tempo, oferecer ao barbeiro uma área onde ele pudesse acompanhar os atendimentos e administrar os serviços.

O sistema foi desenvolvido pensando também na possibilidade de adaptar a aplicação futuramente para outras barbearias ou estabelecimentos que trabalhem com horários.

---

## Funcionalidades

### Agendamento

* Escolha do serviço
* Visualização de preço e duração
* Seleção de data
* Horários disponíveis de acordo com a agenda
* Cadastro do cliente
* Confirmação do agendamento
* Integração com WhatsApp

### Área administrativa

* Login protegido
* Visualização dos agendamentos
* Controle de serviços
* Alteração de preços
* Definição da duração dos serviços
* Controle dos horários de funcionamento
* Controle da agenda
* Acompanhamento financeiro

---

## Tecnologias utilizadas

**Frontend**

* Next.js
* React
* TypeScript
* CSS

**Backend e banco de dados**

* Supabase
* PostgreSQL
* Supabase Auth
* Row Level Security (RLS)

**Integrações e deploy**

* Resend
* Render

---

## Algumas telas

### Página de agendamento

![Página de agendamento](./public/screenshots/agendamento.png)

### Área administrativa

![Dashboard administrativo](./public/screenshots/dashboard.png)

### Visualização no celular

![Versão mobile](./public/screenshots/mobile.png)

---

## Estrutura do projeto

```text
app/
├── admin/
├── api/
└── ...

config/
└── establishment.ts

lib/
├── admin.ts
├── supabase-server.ts
└── supabase.ts

public/

supabase/
└── schema.sql
```

---

## Banco de dados

O projeto utiliza PostgreSQL através do Supabase.

Entre as principais informações armazenadas estão:

* Clientes
* Serviços
* Agendamentos
* Horários
* Configurações da barbearia

O acesso aos dados é protegido utilizando Row Level Security (RLS).

A estrutura inicial do banco está disponível em:

```text
supabase/schema.sql
```

---

## Rodando localmente

Clone o projeto:

```bash
git clone https://github.com/gustavoguga18/saasbarber.git
```

Entre na pasta:

```bash
cd saasbarber
```

Instale as dependências:

```bash
npm install
```

Crie um arquivo `.env.local` com as variáveis do Supabase:

```env
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=
```

Execute o projeto:

```bash
npm run dev
```

Depois acesse:

```text
http://localhost:3000
```

---

## Deploy

A aplicação pode ser publicada no Render.

As variáveis de ambiente devem ser configuradas nas configurações do serviço antes do deploy.

---

## Próximos passos

Algumas melhorias que pretendo continuar implementando:

* Evolução do PWA
* Melhorias na experiência mobile
* Mais opções de notificações
* Relatórios financeiros
* Novas configurações para adaptar o sistema a outros estabelecimentos

---

## Autor

**Gustavo Barbosa**

Projeto desenvolvido como parte do meu aprendizado e prática em desenvolvimento web full-stack.

[GitHub](https://github.com/gustavoguga18)
