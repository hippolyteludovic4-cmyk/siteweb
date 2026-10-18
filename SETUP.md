# Mise en place du projet

Suivi des étapes de configuration : ce qui est fait, ce qui reste à faire, et quand chaque étape devient nécessaire.

Dernière mise à jour : 18 octobre 2026

## Fait

- [x] Dépôt GitHub `siteweb` créé
- [x] Skills Claude installés dans `.claude/skills/` (19 skills, 4 agents)
  - ibelick/ui-skills : `baseline-ui`, `fixing-accessibility`, `fixing-metadata`, `fixing-motion-performance`, `improve-ui`, `create-design-md`, `component-canvas`, `ui-skills-root`
  - pbakaus/impeccable : `impeccable` et ses 4 agents (hooks automatiques non activés)
  - nextlevelbuilder/ui-ux-pro-max : `ui-ux-pro-max`, `design`, `design-system`, `brand`, `banner-design`, `slides`, `ui-styling`
  - microsoft/playwright : `playwright-cli`, `playwright-trace`, `playwright-component-testing`

## À faire

### Maintenant (facultatif)

- [ ] Renommer la branche par défaut en `main` (GitHub → Settings → General → Default branch)

### Au démarrage du projet

- [ ] Définir le projet : type, public, pages, style → `/impeccable init` génère `PRODUCT.md`
- [ ] Choisir la technologie (Next.js pressenti si l'application a une partie serveur)
- [ ] Créer `package.json`, `.gitignore` et installer Playwright (`@playwright/test`)

### Quand l'application a besoin de données ou de comptes utilisateurs

- [ ] Créer un compte [Supabase](https://supabase.com) (connexion via GitHub)
- [ ] Ajouter les clés dans les réglages de l'environnement cloud (menu de l'environnement → Edit → Network secrets, ou variables d'environnement) :
  - `NEXT_PUBLIC_SUPABASE_URL`
  - `NEXT_PUBLIC_SUPABASE_ANON_KEY`
- [ ] Ne jamais coller une clé ou un mot de passe dans la conversation

### Quand on veut mettre le site en ligne

- [ ] Créer un compte [Vercel](https://vercel.com) (connexion via GitHub)
- [ ] Importer le dépôt `siteweb` dans Vercel (déploiement automatique à chaque push)
- [ ] Ajouter les mêmes clés Supabase dans Vercel → Settings → Environment Variables

### Plus tard, selon les besoins

- [ ] Nom de domaine : acheter (OVH, Gandi, Namecheap…) puis le brancher dans Vercel → Settings → Domains
- [ ] Paiements : compte [Stripe](https://stripe.com)
- [ ] E-mails : compte [Resend](https://resend.com)
