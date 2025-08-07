## 🆚 `ng serve` vs `npm start` (Angular)

| Command     | Description                                                                                                                        |
| ----------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| `ng serve`  | Runs your Angular app in development mode using the Angular CLI (usually at `http://localhost:4200`).                              |
| `npm start` | A shortcut for whatever is defined in the `"start"` script in your `package.json`. For Angular projects, it often runs `ng serve`. |

### 🔁 So usually:

```bash
npm start
```

is just an alias for:

```bash
ng serve
```

> ✅ You can check what `npm start` runs by looking inside your `package.json`:

```json
"scripts": {
  "start": "ng serve"
}
```

---

## 🛠️ How to Create a Component in an Existing Folder

Assume you have a folder:

```
src/app/features/dashboard/
```

To create a new component inside it (e.g., `stats` component), run:

```bash
ng generate component features/dashboard/stats
```

or the shorthand:

```bash
ng g c features/dashboard/stats
```

This will create:

```
src/app/features/dashboard/stats/
  ├── stats.component.ts
  ├── stats.component.html
  ├── stats.component.css
  └── stats.component.spec.ts
```

---

Need help choosing a component name or organizing folders better? Just ask.
