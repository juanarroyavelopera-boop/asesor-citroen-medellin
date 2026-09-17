# Asesor Citroën Medellín

Sitio estático generado con la plantilla de marcas que vive en
`asesor-suzuki-medellin-/plantilla`.

**NO se edita a mano.** Los cambios se hacen en la plantilla y se regenera:

    node construir.js citroen ../asesor-citroen-medellin

Tres archivos mandan sobre lo que dice esta página:

    marcas/citroen.json      quién es: dominio, número, medición, modelos
    contenido/citroen.json   qué dice: textos, especificaciones, fotos
    precios/citroen.json     cuánto vale, DE RESPALDO — el CRM manda en vivo

Los precios escritos en el HTML son la red de seguridad: `nucleo/catalogo-vivo.js`
los reemplaza con los del CRM al cargar. Si el CRM no contesta, la página sigue
mostrando precios correctos en vez de quedarse en blanco.
