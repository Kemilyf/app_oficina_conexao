# Conecta Estudos

Aplicativo responsivo para organização dos estudos para concursos públicos.

## Tecnologias
- React 19.3.1
- Vite 8.3.5
- Supabase JS

## Desenvolvimento
```bash
npm install
cp .env.example .env.local
npm run dev
```

Configure `VITE_SUPABASE_URL` e `VITE_SUPABASE_PUBLISHABLE_KEY` com os dados do projeto Supabase. Use somente a chave publicável no navegador; nunca exponha `service_role` ou chaves secretas.

## Build
```bash
npm run build
```

A tabela `public.study_subjects` usa RLS para que cada usuário autenticado acesse apenas suas próprias matérias. O painel possui dados demonstrativos até o login e carregamento dos dados do usuário.
