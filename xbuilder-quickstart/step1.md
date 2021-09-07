XBuilder es una librería Java. Para su uso, recomendamos el uso de [Maven](https://maven.apache.org/) o [Gradle](https://gradle.org/) para la administración de dependencias. En este tutorial aprenderás a crear un proyecto [Maven](https://maven.apache.org/), instalar XBuilder, y finalmente crear tu primer XML producto de una factura electrónica.

## Crea un proyecto Maven

Usaremos el terminal de comandos para crear nuestro proyecto [Maven](https://maven.apache.org/). Haz click en el siguiente comando para ejecutarlo en el terminal.

`mvn archetype:generate -DgroupId=org.openubl.xbuilder -DartifactId=xbuilder-quickstart -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false`{{execute T1}}

> El comando anterior creó un proyecto Maven en la carpeta `xbuilder-quickstart`. Revisa el contenido de la carpeta para familiarizarte con la estructura de un proyecto Maven.

## Configura la versión de Java en tu proyecto Maven

- Abre el archivo `xbuilder-quickstart/pom.xml`{{open}}
- Agrega las las siguientes lineas:

```xml
<properties>
  <maven.compiler.source>1.8</maven.compiler.source>
  <maven.compiler.target>1.8</maven.compiler.target>
</properties>
```{{copy}}

> Los `<properties/>` deben de ser insertados debajo de `<url>http://maven.apache.org</url>`

La versión final debe de ser:

Copy file to editor:

<pre class="file" data-filename="xbuilder-quickstart/pom.xml" data-target="replace">
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/maven-v4_0_0.xsd">
  <modelVersion>4.0.0</modelVersion>
  <groupId>org.openubl.xbuilder</groupId>
  <artifactId>xbuilder-quickstart</artifactId>
  <packaging>jar</packaging>
  <version>1.0-SNAPSHOT</version>
  <name>xbuilder-quickstart</name>
  <url>http://maven.apache.org</url>
  <properties>
    <maven.compiler.source>1.8</maven.compiler.source>
    <maven.compiler.target>1.8</maven.compiler.target>
  </properties>
  <dependencies>
    <dependency>
      <groupId>junit</groupId>
      <artifactId>junit</artifactId>
      <version>3.8.1</version>
      <scope>test</scope>
    </dependency>
  </dependencies>
</project>
</pre>
