# Codex con LLM-proxy

Elegí la descarga correspondiente a tu acceso y hacé clic para
**descargar el ZIP directamente**. La clave va por separado.

## [⬇ Descargar REMOTO para Windows](https://github.com/jpsala/codex-remoto/raw/refs/heads/main/Codex-Remoto-Windows.zip)

Para quienes reciben una **clave REMOTO** de JP. Kit probado en Windows.

## [⬇ Descargar REMOTO para Mac](https://github.com/jpsala/codex-remoto/raw/refs/heads/main/Codex-Remoto-Mac.zip)

**Pendiente de prueba real en macOS.** Coordiná la primera prueba con JP.

## [⬇ Descargar JP para Windows](https://github.com/jpsala/codex-remoto/raw/refs/heads/main/Codex-JP-Windows.zip)

Para las computadoras de JP, con la **clave JP** y acceso completo a los
modelos de Codex del VPS, incluido Astra. Probado en Windows con el CLI y
el motor de la app. No hay kit JP para Mac por ahora.

## Después de descargar

Necesitás tener Codex instalado. Si todavía no lo tenés,
[descargá Codex desde el sitio oficial](https://chatgpt.com/codex) e instalalo primero.

1. **Cerrá Codex y extraé el ZIP.** Buscalo en Descargas. En Windows, clic
   derecho → **Extraer todo**; si usás WinRAR, elegí **Extraer en**.
   No abras el configurador dentro de WinRAR ni desde la vista del ZIP.
   En Mac, doble clic en el ZIP.
2. **Abrí la carpeta extraída y hacé doble clic en el configurador:**
   `Configurar-Remoto.cmd` para REMOTO Windows, `Configurar-Remoto.command`
   para REMOTO Mac o `Configurar-JP.cmd` para JP Windows.
   Pegá la clave de ese acceso cuando te la pida. La entrada es oculta.
3. **Volvé a abrir Codex y creá un chat nuevo.**

REMOTO selecciona **LLM-proxy REMOTO**, con **GPT-6.1 Sol en medium**.
JP selecciona **LLM-proxy JP** y conserva el modelo y esfuerzo anteriores
si son compatibles; en una configuración nueva usa **GPT-6.1 Sol en medium**.
En el CLI podés consultar `/status`; en la app revisá el modelo y, con JP,
el proveedor si la interfaz no lo muestra. En un chat nuevo pedí:

> Responde exactamente: gateway-ok

Después pedí `Responde exactamente: segundo-ok`. Una respuesta aislada no
identifica la ruta: si hay dudas, JP debe comprobar la configuración y el gateway.

## Modelos y acceso

**REMOTO:** GPT-6.1 Sol, GPT-6 Sol, GPT-6 Luna, GPT-5.6 Sol, GPT-5.6 Terra,
GPT-5.6 Luna y GPT-5.5, con esfuerzo **low, medium o high**, sin Astra.

**JP:** todos los modelos de Codex disponibles en el VPS, incluido Astra,
y todos los esfuerzos que admita cada modelo. Los modelos de imagen de la
API no aparecen como opciones de conversación en Codex.

Ambos accesos usan el VPS de JP y comparten el cupo de su cuenta. La clave
JP es distinta de REMOTO; la clave administrativa del panel no sirve para
estos kits. Ninguna clave viene incluida en las descargas.

La clave se guarda en el **Llavero de macOS** o cifrada con **DPAPI de Windows**
para tu usuario. No necesitás Tailscale, Bun, Node, Python ni un proxy local.
Cada computadora se configura por separado; no copies carpetas `.codex`,
archivos de claves ni respaldos entre equipos. No compartas la clave con terceros.

## Ayuda

En Mac, si el doble clic no abre el configurador, abrí Terminal, escribí
`/bin/bash` y un espacio, arrastrá `Configurar-Remoto.command` y presioná Enter.

Si algo falla, avisale a JP el sistema, la versión de Codex y el paso donde
falló, con el mensaje de error sin datos privados. No publiques claves,
configuraciones completas ni respaldos en GitHub.

El `LEEME.txt` dentro de cada ZIP explica dónde queda el respaldo para volver
atrás con ayuda de JP. Los [SHA-256](SHA256SUMS.txt) permiten verificar que
los archivos descargados coinciden con esta entrega. También podés leer
la [guía completa](LEEME.txt).
