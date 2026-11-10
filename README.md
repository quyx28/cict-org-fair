# CICT Org Fair

Flutter Web app for the CICT organization fair. Event data is loaded from
Contentful's Content Delivery API.

Live Web app: https://quyx28.github.io/cict-org-fair/

## Contentful configuration

Create a local `cms.json` file from `cms.example.json` and replace the
placeholder values with a Contentful Space ID and a read-only Content Delivery
API token. `cms.json` is ignored by Git.

Run locally:

```powershell
flutter run -d chrome --dart-define-from-file=cms.json
```

Build for deployment:

```powershell
flutter build web --dart-define-from-file=cms.json
```

Only use a Contentful delivery token. Never put a Content Management token in
the app.
