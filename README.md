![Decal_Video](https://github.com/user-attachments/assets/c4e86f74-e134-4b7f-9791-22ebd9b2fb76)

# Decals

Proyecto de **sistema de decals en Unity 6 (URP)**, pensado como base clara y reutilizable para impactos, suciedad, señales y detalles visuales sobre superficies.

![Banner](https://github.com/user-attachments/assets/5b933a56-0ece-452a-99c0-1a641485a6b9)

## ✨ ¿Qué ofrece este repositorio?

- Escena(s) de ejemplo para experimentar con decals en un entorno real.
- Configuración orientada a **Universal Render Pipeline (URP)**.
- Estructura de carpetas organizada para escalar el proyecto.
- Base preparada para evolucionar a paquete distribuible.

## 🧱 Stack técnico

- **Unity:** `6000.3.10f1` (Unity 6)
- **Render Pipeline:** `com.unity.render-pipelines.universal` `17.3.0`
- **VFX Graph:** `com.unity.visualeffectgraph` `17.3.0`

## 📋 Requisitos

Antes de abrir el proyecto, asegúrate de tener:

1. **Unity Hub** instalado.
2. Editor **Unity 6000.3.10f1**.
3. Conexión a Internet para restaurar dependencias de paquetes al primer import.

## 🚀 Puesta en marcha rápida

1. Clona el repositorio:

   ```bash
   git clone https://github.com/<tu-usuario>/Decals.git
   ```

2. Abre **Unity Hub** → **Add project** → selecciona la carpeta del repositorio.
3. Verifica que Unity use la versión `6000.3.10f1`.
4. Espera a que Unity termine la importación inicial.
5. Abre una escena de ejemplo desde `Assets/3-Scenes`.

## 🗂️ Estructura del proyecto

```text
Assets/
 ├─ 1-Programming/    # Scripts y lógica (si aplica)
 ├─ 2-Art/            # Materiales, texturas, modelos y recursos visuales
 ├─ 3-Scenes/         # Escenas de ejemplo y pruebas
 ├─ 4-Presets/        # Presets reutilizables
 └─ 5-Settings/       # Configuraciones del proyecto y render

Packages/
 ├─ manifest.json
 └─ packages-lock.json

ProjectSettings/
```

## 🧪 Flujo de uso recomendado

- Duplica una escena de `Assets/3-Scenes` para trabajar sin romper la base.
- Mantén los recursos artísticos en `Assets/2-Art`.
- Si añades lógica de decals, centralízala en `Assets/1-Programming`.
- Crea presets reutilizables para materiales y parámetros frecuentes.

## 📦 Publicación (GitHub Actions)

El repositorio incluye un workflow (`.github/workflows/publish.yml`) para publicación en npm al crear un release.

> Nota: actualmente el workflow espera una ruta `Packages/com.jaimecamacho.<repo>/package.json`. Si vas a publicar como paquete, crea esa estructura o ajusta el workflow antes de generar el release.

## 🤝 Contribuciones

Las contribuciones son bienvenidas.

1. Crea una rama desde `main`.
2. Haz commits pequeños y descriptivos.
3. Abre un Pull Request explicando claramente:
   - Problema o necesidad.
   - Solución aplicada.
   - Pasos para validar.

## 📄 Licencia

Este proyecto se distribuye bajo licencia **MIT**. Revisa el archivo [LICENSE](./LICENSE).

---

Si quieres, puedo convertir este README en una versión enfocada a **usuarios finales** (uso rápido) o en otra orientada a **desarrolladores del paquete** (arquitectura + API + roadmap).
