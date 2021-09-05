- Crea un proyecto Maven usando el comando:

`mvn archetype:generate -DgroupId=org.openubl.xbuilder -DartifactId=xbuilder-quickstart -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false`{{execute T1}}

- El comando anterior creó un proyecto maven en la carpeta `xbuilder-quickstart`. Revisa el contenido de la carpeta.
- Configura la versión de Java:

Agrega las siguientes lineas debajo de `<url>http://maven.apache.org</url>`:

```xml
 <properties>
  <maven.compiler.source>1.8</maven.compiler.source>
  <maven.compiler.target>1.8</maven.compiler.target>
</properties>
```

### Notas adicionales

Puedes utilizar el método de tu preferencia para inicializar un proyecto hecho en maven. Te sugerimos leer la documentación [creating-a-proyect-in-maven](https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html#creating-a-project)
