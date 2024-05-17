Este é um projeto incrível construído com Next.js.
Ele foi construído usando Mysql como banco de dados,
Clerk como solução de autenticação,
Uploadthing como host de imagens,
Prisma como solução ORM e
Livekit como solução de web-sharing.
Para executá-lo em sua máquina local, siga estas etapas:

**Clone o repositório:**
git clone https://github.com/PedroML71/discord-clone.git

**Instale as dependências:**
npm install

**Crie um arquivo `.env` na raiz do projeto:**

**Adicione as seguintes variáveis de ambiente ao arquivo `.env`:**
DATABASE_URL=seu-url-do-banco-de-dados
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=chave-publica-do-clerk
CLERK_SECRET_KEY=chave-secreta-do-clerk
NEXT_PUBLIC_CLERK_SIGN_IN_URL=link-login-do-app (no caso deste app você deve usar o /sign-in)
NEXT_PUBLIC_CLERK_SIGN_UP_URL=link-cadastro-do-app (no caso deste app você deve usar o /sign-up)
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=link-redirect-após-login (no caso deste app você deve usar o /)
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=link-redirect-após-cadastro (no caso deste app você deve usar o /)
UPLOADTHING_SECRET=senha-secreta-do-uploadthing
UPLOADTHING_APP_ID=id-do-projeto-seu-projeto-uploadthing
LIVEKIT_API_KEY=id-do-projeto-livekit
LIVEKIT_API_SECRET=senha-secreta-do-projeto-livekit
NEXT_PUBLIC_LIVEKIT_URL=url-wss-póblica-do-projeto-livekit

**Inicie o prisma:**
npx prisma db push

**Inicie o servidor de desenvolvimento:**
npm run dev
