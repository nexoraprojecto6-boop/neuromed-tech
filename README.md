# NEUROMED

**Status:** Architecture / Initial Structure

## Objective
NEUROMED is a digital health platform connecting patients and professionals
(appointments, video sessions, messaging, subscriptions, content and wellness tracking).

## Architecture
Monorepo with three applications (mobile, API, admin) sharing internal packages.
Domain-oriented modules, with privacy and security folders prepared from day one.

## Monorepo structure
- `apps/mobile` - React Native + Expo
- `apps/api` - NestJS + Prisma + PostgreSQL
- `apps/admin` - Next.js admin dashboard
- `packages/*` - shared types, ui, config, validation, database, utils
- `docs/` - architecture, api, database, product and security docs
- `infrastructure/` - docker, nginx, scripts
- `.github/workflows` - CI and security pipelines (placeholders)

## Planned stack
pnpm workspaces, Node.js, TypeScript, React Native/Expo, NestJS, Prisma,
PostgreSQL, Next.js. Future: Redis, file storage, e-mail, push notifications,
video provider, payment gateway.
