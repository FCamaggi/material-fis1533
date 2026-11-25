# FIS1533 Electricidad y Magnetismo (UC) · Material reunido

Clases, ayudantías, pruebas anteriores y material de apoyo del curso FIS1533 de la Pontificia Universidad Católica de Chile, ordenado para descargar lo que necesites. Casi todos los PDF tienen su transcripción en Markdown en una subcarpeta `markdown/`.

**Guía de estudio para el examen 2026-2:** https://fcamaggi.github.io/guia-estudio-examen-fis1533/

> Este material es de sus autores (profesores, ayudantes y estudiantes que lo compartieron). Aquí solo está reunido y ordenado, para estudiar. Lee [CREDITOS.md](CREDITOS.md) antes de redistribuirlo.

## Qué hay y dónde

| Carpeta | Qué contiene |
| --- | --- |
| [`pruebas-anteriores/`](pruebas-anteriores/README.md) | **Todas las pruebas en un solo lugar:** I1, I2, I3, exámenes, controles y tareas desde 2010 hasta 2026-2, con pautas. Una sola copia de cada archivo y una tabla por semestre. |
| [`material-apoyo/`](material-apoyo/README.md) | Apuntes y libro de Fabián Cádiz, compilados de problemas (Benguria, Chi, Urrutia), resúmenes, masivas del Proyecto GOING, repasos de otras secciones, tips de SalvaRamos y ayudantías 2022-2. |
| [`2026-2/`](2026-2/README.md) | Semestre en curso: clases 02–14 y ayudantías 01–28 (las 01–25 con transcripción completa: LaTeX y descripción de figuras), programa y temario del examen. |
| [`2026-1/`](2026-1/README.md) | Prof. Rodrigo López: unidades 1–4 y ayudantías 00–30. |
| [`2025-2/`](2025-2/README.md) | Prof. Macarena Domínguez: clases, ayudantías 01–30, mini controles formativos, guías y resúmenes. |
| [`2024-2/`](2024-2/README.md) | Prof. Giuseppe De Nittis: ayudantías y `Contenidos.md` con las páginas de la bibliografía por clase. |

## Cómo descargar solo lo que quieres

- **Un archivo:** ábrelo en GitHub y usa *Download raw file*.
- **Todo:** botón *Code → Download ZIP* (pesa alrededor de 1 GB).
- **Una carpeta** (por ejemplo, solo las pruebas):

  ```bash
  git clone --filter=blob:none --sparse <url-del-repositorio>
  cd <carpeta-del-repositorio>
  git sparse-checkout set pruebas-anteriores
  ```

## Sobre las transcripciones en Markdown

- **Mejor calidad:** las clases y ayudantías de 2026-2 y las pautas oficiales desde 2024-2 (en `pruebas-anteriores/*/markdown/`) se transcribieron con IA multimodal: ecuaciones en LaTeX y figuras descritas como `[Figura]`.
- **El resto** se extrajo con `pdftotext` y se limpió; puede tener fórmulas rotas. Los PDF escaneados o manuscritos sin capa de texto aparecen en las tablas sin Markdown.
- Ante cualquier diferencia, manda el PDF original.

## Para agentes de IA

- Lee primero los `README.md` de cada carpeta: listan cada archivo con su extensión y su par Markdown.
- Prefiere los `.md` a los PDF; para pruebas, usa la tabla por semestre de `pruebas-anteriores/README.md`.
- `*/scratch/` no se publica: son imágenes intermedias de la transcripción.

## Nombres de archivo en `pruebas-anteriores/`

`<Tipo> <Año>-<Semestre> (<variante>).pdf`, por ejemplo `I2 2025-2 (pauta).pdf`. Sin variante es el enunciado. La lista de variantes está en [`pruebas-anteriores/README.md`](pruebas-anteriores/README.md).
