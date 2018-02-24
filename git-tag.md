# git tag
Lista las etiquetas existentes

## git tag nombre_etiqueta
Lista las etiquetas en orden alfabetico.

## git tag -a nombre_etiqueta -m "mensaje de la etiqueta"

Etiqueta anotada. Se guardan en la base de datos de git como un objeto entero.

```
git tag -l "v1.*"
```

Lista las etiquetas que coincidan con el patron especificado.