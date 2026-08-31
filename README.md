# VR_VLIR

Proyecto de **Realidad Virtual** desarrollado con **Unreal Engine 5.7.4** para dispositivos **Meta Quest**.

El proyecto utiliza **Meta XR + OpenXR** para las funcionalidades de realidad virtual.

---

## 📋 Requisitos

Antes de abrir el proyecto necesitas instalar:

- **Unreal Engine 5.7.4**
- **Meta XR Plugin** compatible con Unreal Engine 5.7.4
- **Android Studio**
- **Android SDK**
- **Android NDK**
- **Java/JDK compatible con Unreal Engine 5.7.4**
- **Git**
- **Git LFS**

### Hardware

- PC con Windows 10/11
- GPU compatible con Unreal Engine y VR
- Meta Quest compatible
- Cable USB-C para desarrollo o conexión inalámbrica compatible

---

# 🎮 Unreal Engine 5.7.4

Este proyecto fue desarrollado utilizando:

**Unreal Engine 5.7.4**

Se recomienda utilizar exactamente esta versión del motor para evitar problemas de compatibilidad con:

- Blueprints
- Plugins
- Assets
- Materiales
- Configuración de Android
- Meta XR
- OpenXR

Descarga Unreal Engine desde:

https://www.unrealengine.com/download

También puedes instalarlo mediante **Epic Games Launcher**.

---

# 🥽 Meta XR Plugin

El proyecto utiliza **Meta XR Plugin para Unreal Engine**.

> **IMPORTANTE:** El Meta XR Plugin **no está incluido en este repositorio** y debe instalarse por separado.

### Documentación oficial

https://developers.meta.com/horizon/documentation/unreal/unreal-quick-start-install-metaxr-plugin/

### Descargas oficiales

https://developers.meta.com/horizon/downloads/

---

## ⚠️ Compatibilidad de Meta XR

**IMPORTANTE**

Este proyecto utiliza:

```text
Unreal Engine 5.7.4
```

La versión de Meta XR utilizada debe ser compatible con **Unreal Engine 5.7.4**.

La documentación actual de Meta indica que el plugin descargable está dirigido a la versión más reciente soportada de Unreal Engine. Para otras versiones de Unreal Engine, Meta recomienda utilizar el plugin correspondiente desde el fork Oculus-VR de Unreal Engine.

Por lo tanto:

> **No instales automáticamente la última versión de Meta XR sin comprobar primero su compatibilidad con Unreal Engine 5.7.4.**

Documentación oficial:

https://developers.meta.com/horizon/documentation/unreal/unreal-quick-start-install-metaxr-plugin/

---

# 📥 Instalación de Meta XR

## 1. Descargar Meta XR

Abre:

https://developers.meta.com/horizon/downloads/

Busca la integración:

```text
Unreal Engine 5 Integration
```

Descarga la versión de Meta XR compatible con tu versión de Unreal Engine.

Meta indica que el plugin descargable se distribuye como un archivo `.zip`.

---

## 2. Extraer el plugin

Extrae el contenido del `.zip`.

La documentación oficial de Meta indica que, para una instalación normal de Unreal Engine, el plugin debe colocarse en:

```text
[UNREAL_ENGINE]\Engine\Plugins\Marketplace
```

Por ejemplo:

```text
C:\Program Files\Epic Games\UE_5.7\Engine\Plugins\Marketplace
```

Si la carpeta `Marketplace` no existe, créala.

Fuente oficial:

https://developers.meta.com/horizon/documentation/unreal/unreal-quick-start-install-metaxr-plugin/

---

## 3. Activar Meta XR

Abre Unreal Engine y carga el proyecto.

Ve a:

```text
Edit
→ Plugins
```

Busca:

```text
Meta XR
```

Comprueba que aparezca instalado.

Si está desactivado, actívalo:

```text
Enabled
```

Reinicia Unreal Engine si se solicita.

---

# 📱 Android / Meta Quest

Para compilar y ejecutar el proyecto en Meta Quest también necesitas configurar Android.

Instala:

### Android Studio

https://developer.android.com/studio

Después configura:

- **Android SDK**
- **Android NDK**
- **Java/JDK**

Estos componentes deben ser compatibles con **Unreal Engine 5.7.4**.

Documentación oficial de Meta:

https://developers.meta.com/horizon/documentation/unreal/unreal-quick-start-setup-dev-environ/

---

# 🥽 Configurar Meta Quest

Para ejecutar el proyecto directamente en un Meta Quest:

1. Configura el visor para desarrollo.
2. Activa el modo desarrollador.
3. Conecta el Quest al PC mediante USB-C o utiliza una conexión inalámbrica compatible.
4. Abre Unreal Engine.
5. Comprueba que Meta XR esté habilitado.
6. Comprueba la configuración de Android.
7. Ejecuta el proyecto o genera un APK.

Documentación oficial:

https://developers.meta.com/horizon/documentation/unreal/

---

# 📦 Clonar el proyecto

Instala Git:

https://git-scm.com/download/win

Instala Git LFS:

```powershell
git lfs install
```

Clona el repositorio:

```powershell
git clone https://github.com/JohnnyBarrenoU/VR_VLIR.git
```

Entra en la carpeta:

```powershell
cd VR_VLIR
```

Descarga los archivos almacenados mediante Git LFS:

```powershell
git lfs pull
```

---

# 🚀 Abrir el proyecto

Después de clonar el repositorio:

1. Instala **Unreal Engine 5.7.4**.
2. Instala **Meta XR compatible con UE 5.7.4**.
3. Instala y configura **Android Studio**.
4. Ejecuta:

```text
VR_VLIR.uproject
```

5. Abre el proyecto con **Unreal Engine 5.7.4**.
6. Comprueba que **Meta XR** esté habilitado.

---

# 🗂️ Estructura del proyecto

La estructura principal es:

```text
VR_VLIR/
│
├── Config/
├── Content/
├── DisabledPlugins/
├── Plugins/
├── Script/
│
├── .gitattributes
├── .gitignore
├── README.md
│
└── VR_VLIR.uproject
```

Las siguientes carpetas no se almacenan en Git porque Unreal Engine las genera automáticamente:

```text
Binaries/
Intermediate/
Saved/
DerivedDataCache/
```

No es necesario descargarlas manualmente.

---

# 🧩 Plugins

Los plugins incluidos específicamente dentro del proyecto se encuentran en:

```text
Plugins/
```

Actualmente esta carpeta puede estar vacía porque algunos plugins utilizados por el proyecto pueden estar instalados a nivel del Unreal Engine.

### Meta XR

Meta XR debe instalarse manualmente siguiendo las instrucciones oficiales de Meta.

No es necesario copiar toda la carpeta:

```text
Engine/Plugins/
```

al proyecto.

Solo deben instalarse los plugins requeridos.

---

# 🔄 Actualizar el proyecto

Si ya clonaste el proyecto y quieres obtener los últimos cambios:

```powershell
git pull
git lfs pull
```

---

# 📤 Subir cambios

Después de modificar el proyecto:

```powershell
git add .
```

Crea un commit:

```powershell
git commit -m "Descripción de los cambios"
```

Sube los cambios:

```powershell
git push
```

---

# 🌿 Crear una rama

Para trabajar en una nueva funcionalidad:

```powershell
git checkout -b desarrollo
```

Después:

```powershell
git add .
git commit -m "Nueva funcionalidad"
git push -u origin desarrollo
```

---

# ⚠️ Problemas comunes

## Unreal indica que falta Meta XR

Ve a:

```text
Edit → Plugins
```

y busca:

```text
Meta XR
```

Si no aparece, instala el plugin siguiendo la documentación oficial:

https://developers.meta.com/horizon/documentation/unreal/unreal-quick-start-install-metaxr-plugin/

---

## Faltan archivos después de clonar

Ejecuta:

```powershell
git lfs install
git lfs pull
```

---

## Unreal solicita recompilar

Si Unreal solicita recompilar módulos del proyecto o de un plugin, permite la compilación siempre que los módulos correspondan a la versión de Unreal Engine utilizada.

---

# 🔗 Documentación

### Meta XR Plugin

https://developers.meta.com/horizon/documentation/unreal/unreal-quick-start-install-metaxr-plugin/

### Meta XR Downloads

https://developers.meta.com/horizon/downloads/

### Configuración del entorno

https://developers.meta.com/horizon/documentation/unreal/unreal-quick-start-setup-dev-environ/

### Unreal Engine

https://www.unrealengine.com/

### Android Studio

https://developer.android.com/studio

### Git

https://git-scm.com/download/win

---

# 📌 Información del proyecto

| Elemento | Versión |
|---|---|
| Unreal Engine | **5.7.4** |
| Plataforma | **Meta Quest / Android** |
| XR | **Meta XR + OpenXR** |
| Control de versiones | **Git + Git LFS** |

---

## 👤 VR_VLIR

Proyecto de realidad virtual desarrollado en **Unreal Engine 5.7.4** para **Meta Quest**.