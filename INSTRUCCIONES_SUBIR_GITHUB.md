# 📋 Instrucciones para subir a GitHub

## Paso 1 — Organizá tu carpeta en el escritorio

Creá una carpeta llamada `Furniture-Solutions-PowerBI` en tu escritorio
y copiá adentro estos archivos:

```
Furniture-Solutions-PowerBI/
│
├── README.md                                    ✅ (este archivo ya está)
├── .gitignore                                   ✅ (ya está)
├── Furniture_Solutions_M_N_co.pbix              ← copiá desde tu escritorio
├── stores_sales_forecasting.xlsx                ← copiá desde tu escritorio
├── DS1_Matias_Nicolas_Diaz.ipynb                ← copiá desde tu escritorio
│
├── docs/
│   ├── Documentacion_Furniture_Solutions_M_N_co_Entrega_Final.pdf
│   └── Storytelling.pdf
│
└── img/
    └── (sacá una captura de pantalla del dashboard y guardala como dashboard_preview.png)
```

---

## Paso 2 — Creá el repositorio en GitHub

1. Andá a https://github.com
2. Hacé click en **"New repository"** (botón verde)
3. Completá:
   - **Repository name:** `Furniture-Solutions-PowerBI`
   - **Description:** `Sales Analysis Dashboard (2014-2017) | Power BI + Python | ABC Pareto, DAX, ML`
   - **Visibility:** Public ✅
   - **⚠️ NO marques** "Add a README file"
4. Hacé click en **"Create repository"**

---

## Paso 3 — Subí los archivos desde la terminal

Abrí PowerShell en tu carpeta del proyecto y ejecutá estos comandos uno por uno:

```powershell
# 1. Inicializá git
git init

# 2. Configurá tu usuario (solo la primera vez)
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"

# 3. Agregá todos los archivos
git add .

# 4. Hacé el primer commit
git commit -m "Initial commit - Furniture Solutions Sales Dashboard"

# 5. Conectá con GitHub (reemplazá TU_USUARIO con tu usuario de GitHub)
git remote add origin https://github.com/TU_USUARIO/Furniture-Solutions-PowerBI.git

# 6. Subí los archivos
git branch -M main
git push -u origin main
```

---

## Paso 4 — Verificá en GitHub

Entrá a `https://github.com/TU_USUARIO/Furniture-Solutions-PowerBI`
y deberías ver el README renderizado con toda la info del proyecto. ✅

---

## ⚠️ Nota sobre archivos grandes

GitHub tiene un límite de **25 MB por archivo** en la interfaz web
y **100 MB** por git push normal.

Si el `.pbix` o el `.xlsx` son muy grandes, tenés dos opciones:
- Subir el archivo manualmente desde la interfaz web de GitHub (arrastrando)
- Usar **Git LFS** (Large File Storage): `git lfs track "*.pbix"`

---

## 💡 Tip extra: Captura del dashboard

Para sacar la captura del dashboard:
1. Abrí el `.pbix` en Power BI Desktop
2. Apretá `Windows + Shift + S` para capturar la pantalla
3. Guardá como `dashboard_preview.png` en la carpeta `img/`

Esto hace que el README se vea mucho mejor en GitHub. 🎨
