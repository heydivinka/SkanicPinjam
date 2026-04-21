# Deployment Steps

## [ ] 1. Edit composer.json
Add `"platform-check": false` to config section.

## [ ] 2. Git commit
```bash
git add composer.json
git commit -m "fix: disable platform-check for Railway deploy"
git push origin main
```

## [ ] 3. Railway Dashboard
- Replace railway.toml with railway-fixed.toml
- Add DB vars (MYSQL*)
- Add APP_KEY from `php artisan key:generate --show`
- Redeploy

## [ ] 4. Run migrations
```
railway run php artisan migrate --seed
```

## [ ] 5. Live!

