# Experiencia WebAR con Marcador NFT — Modelo 3D Árbol

Proyecto de **Realidad Aumentada en la web (WebAR)** desarrollado con **A-Frame** y **AR.js**, basado en reconocimiento de imagen natural (**NFT – Natural Feature Tracking**). Al apuntar la cámara web o del dispositivo móvil hacia la imagen marcador, la aplicación superpone en tiempo real un modelo tridimensional (`arbol.glb`) sobre la superficie detectada.

---

## Características principales

* **Rastreo sin marcadores fiduciales (NFT):** Reconocimiento directo de características visuales de una fotografía o ilustración mediante descriptores `.fset`, `.fset3` e `.iset`.
* **Visualización 3D en navegador:** Renderizado en tiempo real con iluminación ambiental y direccional mediante `A-Frame 1.4.2` y `AR.js`, sin necesidad de instalar aplicaciones externas.
* **Interfaz de estado y calibración en vivo:**
  * Indicador visual dinámico que informa si la cámara está buscando el objetivo o si el marcador fue detectado.
  * Panel desplegable (**Ajustes 3D**) para modificar en tiempo real la escala, posición ($X, Y, Z$) y rotación del modelo sobre el marcador.

---

## Estructura del repositorio

```text
├── index.html        # Escena A-Frame/AR.js, lógica de rastreo e interfaz de usuario
├── arbol.glb         # Modelo 3D en formato glTF binario
├── marcador.fset     # Descriptores de características del marcador NFT
├── marcador.fset3    # Descriptores de seguimiento 3D del marcador NFT
├── marcador.iset     # Conjunto de imágenes piramidales del marcador NFT
├── foto.jpg          # Imagen de referencia utilizada como marcador físico/digital
└── README.md         # Documentación del proyecto
