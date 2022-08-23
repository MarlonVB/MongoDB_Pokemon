# Utilice di.find () como la instrucción SQL LIKE

Puede utilizar expresiones regulares para buscar documentos en Monogdb. Esto será similar a las declaraciones LIKE en las consultas SQL.

* _**Cadena de búsqueda en todas partes:**_
Monogdb permite utilizar expresiones regulares para buscar archivos. Esto es similar a una sentencia LIKE en una consulta SQL.

```
db.data.find({campo: /t/})

```

* _**Cadena de búsqueda comienza con:**_
Se mostrar todas aquellas cuya letra comience con la letra especificada, la sintaxis es la siguiente:

```
db.data.find({campo: /^t/})

```

* _**Buscar al final de una cadena:**_
El carácter $ se utiliza para evaluar si el final de una cadena con un carácter específico, la sintaxis es la siguiente:

```
db.data.find({campo: /t$/})

```
