 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
new file mode 100644
index 0000000000000000000000000000000000000000..1cb17559f06312330c778ec30cc1d3147b744ec0
--- /dev/null
+++ b/README.md
@@ -0,0 +1,18 @@
+# lab2026
+
+<p align="center">
+  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:2563eb&height=220&section=header&text=LAB2026&fontSize=56&fontColor=ffffff&animation=fadeIn" alt="Banner principal de lab2026" />
+</p>
+
+Bienvenido a **lab2026** 👋
+
+## Descripción
+Este repositorio está preparado como laboratorio para pruebas, experimentación y documentación del proyecto.
+
+## Estructura inicial
+- `README.md`: documentación principal del proyecto.
+

EOF
)
