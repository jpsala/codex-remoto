# Codex REMOTO

Elegí tu computadora y hacé clic para **descargar el ZIP directamente**.
JP te pasa la clave de acceso por separado.

## [⬇ Descargar para Windows](https://github.com/jpsala/codex-remoto/raw/refs/heads/main/Codex-Remoto-Windows.zip)

Kit probado en Windows. Al terminar la descarga, seguí los tres pasos de abajo.

## [⬇ Descargar para Mac](https://github.com/jpsala/codex-remoto/raw/refs/heads/main/Codex-Remoto-Mac.zip)

**Pendiente de prueba real en macOS.** Coordiná la primera prueba con JP.

## Después de descargar

Necesitás tener Codex instalado. Si todavía no lo tenés,
[descargá Codex desde el sitio oficial](https://chatgpt.com/codex) e instalalo primero.

1. **Cerrá Codex y extraé el ZIP.** Buscalo en Descargas. En Windows, clic
   derecho → **Extraer todo**. En Mac, doble clic en el ZIP.
2. **Abrí la carpeta extraída y hacé doble clic en el configurador:**
   `Configurar-Remoto.cmd` en Windows o `Configurar-Remoto.command` en Mac.
   Pegá la clave que te pasó JP cuando te la pida. La entrada es oculta.
3. **Volvé a abrir Codex y creá un chat nuevo.**

Queda seleccionado **LLM-proxy REMOTO**, con **GPT-6.1 Sol en medium**.
En el CLI podés consultar `/status`; en la app revisá el modelo y, con JP,
el proveedor si la interfaz no lo muestra. En un chat nuevo pedí:

> Responde exactamente: gateway-ok

Después pedí `Responde exactamente: segundo-ok`. Una respuesta aislada no
identifica la ruta: si hay dudas, JP debe comprobar la configuración y el gateway.

## Modelos y acceso

Podés elegir GPT-6.1 Sol, GPT-6 Sol, GPT-6 Luna, GPT-5.6 Sol, GPT-5.6 Terra,
GPT-5.6 Luna y GPT-5.5, con esfuerzo **low, medium o high**. Astra queda excluido.
El acceso usa el VPS de JP y comparte el cupo de su cuenta.

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
