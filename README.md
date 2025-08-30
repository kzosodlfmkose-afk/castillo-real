# 🏰 Castillo Real con Guardias y Libro Mágico

## Despliegue Real (Vercel + Clerk)

### 1. Crear aplicación en Clerk
- Ir a https://dashboard.clerk.com/ → New Application
- Copiar las llaves mágicas:
  - NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY
  - CLERK_SECRET_KEY

### 2. Configurar Vercel
En Project Settings → Environment Variables:
```
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_...
CLERK_SECRET_KEY=sk_...
```

### 3. Subir a GitHub y Vercel
- Subir este cofre completo a su repositorio GitHub.
- Importar en Vercel → Deploy.

### 4. Coronar al Rey
- En Clerk Dashboard → Users → tu usuario → `publicMetadata.role = "rey"`

### 5. Entrar al castillo
- Plaza pública: `/`
- Salón del Rey: `/admin` (solo rol "rey")
- Libro Mágico: listado de visitantes y correos en el panel real.
