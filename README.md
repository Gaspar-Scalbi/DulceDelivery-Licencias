# Dulce Delivery Rosario — Licencias

Este repositorio **no contiene código fuente** ni datos legibles.

Aloja archivos de licencia **cifrados**, para que el sistema instalado en la PC de
cada cliente pueda recibir su renovación automáticamente, sin que nadie tenga que
copiar y pegar claves.

## Cómo está protegido

| Capa | Qué hace |
|---|---|
| Nombre del archivo | Es un hash SHA256, así que no se puede saber ni enumerar a quién corresponde cada licencia. |
| Contenido | Cifrado con AES. La clave se deriva del identificador de la máquina de destino: **sólo esa PC puede leer su propio archivo**. |
| Firma | Cada licencia está firmada con RSA-2048. Una licencia no firmada por el proveedor no es aceptada por el sistema, y no sirve en otra máquina. |

En resumen: el contenido de este repositorio no le sirve a nadie más que a la PC
para la que fue emitido.

---

Dulce Delivery Rosario · Gaspar Scalbi