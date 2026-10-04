# Codex REMOTO

Configurá Codex en otra computadora para usar el acceso REMOTO que te entrega JP.
Necesitás tener instalada la app oficial de Codex o el CLI y recibir la clave
REMOTO por separado. Los kits no incluyen claves ni instalan programas.

## Descargar

| Equipo | Kit | Estado |
| --- | --- | --- |
| Windows | [Descargar Codex-Remoto-Windows.zip](Codex-Remoto-Windows.zip) | Probado con CLI y motor de la app |
| Mac | [Descargar Codex-Remoto-Mac.zip](Codex-Remoto-Mac.zip) | Pendiente de prueba real en macOS; primera prueba acompañada por JP |

En GitHub, abrí el archivo y usá **Download raw file** para descargarlo.
También está la [guía completa](LEEME.txt), incluida en esta distribución.

## Configurar

1. Cerrá Codex y extraé el ZIP completo.
2. Abrí `Configurar-Remoto.cmd` en Windows o `Configurar-Remoto.command` en Mac.
3. Pegá la clave REMOTO cuando la pida el configurador. La entrada es oculta.
4. Cuando termine, abrí Codex y creá un chat nuevo.

Si todavía no tenés Codex, descargalo desde [el sitio oficial](https://chatgpt.com/codex).
En Mac, si el doble clic no abre el archivo, abrí Terminal, escribí `/bin/bash`
y un espacio, arrastrá `Configurar-Remoto.command` y presioná Enter.

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

Si algo falla, avisale a JP el sistema, la versión de Codex y el paso donde
falló, con el mensaje de error sin datos privados. No publiques claves,
configuraciones completas ni respaldos en GitHub.

El `LEEME.txt` dentro de cada ZIP explica dónde queda el respaldo para volver
atrás con ayuda de JP. Los [SHA-256](SHA256SUMS.txt) permiten verificar que
los archivos descargados coinciden con esta entrega.
