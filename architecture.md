# L’Architecte : 3 principes d’organisation du projet

Dans le cadre du projet **SénSanté**, l’Architecte joue un rôle central dans l’organisation technique et collaborative de l’équipe. Trois principes structurent son action :

## 1. Gestion technique et qualité du code

L’Architecte établit des standards stricts pour garantir la maintenabilité et la fiabilité du code :
- Adoption de conventions claires basées sur **Next.js / TypeScript**.
- Mise en place de **branches isolées par fonctionnalité** et de **pull requests obligatoires** pour chaque fusion.
- Documentation des patterns réutilisables et revue de code régulière.

## 2. Maîtrise des risques techniques

Il anticipe et mitige les risques identifiés dans le document de vision :
- **API Groq** : mise en place d’un mode dégradé en cas d’indisponibilité, timeout à 10 secondes.
- **Sécurité** : les clés API sont stockées dans `.env` exclusivement, avec interdiction de commit sur GitHub.
- **Déploiement** : configuration précoce de **Docker Compose** et tests réguliers sur tous les environnements.

## 3. Cadrage et animation de l’équipe

L’Architecte garantit le respect du périmètre et la cohésion de l’équipe :
- **Périmètre verrouillé** : toute demande d’évolution hors du document de vision est soumise à validation.
- **Accompagnement technique** : labs progressifs sur Next.js, support pour les membres en difficulté.
- **Transparence** : rapports individuels après chaque lab, suivi via l’historique Git et entraide encouragée.

Ces trois principes assurent une organisation rigoureuse, à la fois technique et humaine, pour livrer une application fiable, sécurisée et conforme aux besoins des agents de santé communautaire.