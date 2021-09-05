- Abre el archivo `xbuilder-quickstart/pom.xml`
- Agrega la dependencia dentro del tag `<dependencies>`:

```xml
<dependency>
    <groupId>io.github.project-openubl</groupId>
    <artifactId>xbuilder</artifactId>
    <version>1.2.1.Final</version>
</dependency>
```{{copy}}

Las dependencias deben de queda así:

```xml
<dependencies>
  <dependency>
    <groupId>junit</groupId>
    <artifactId>junit</artifactId>
    <version>3.8.1</version>
    <scope>test</scope>
  </dependency>
  <dependency>
    <groupId>io.github.project-openubl</groupId>
    <artifactId>xbuilder</artifactId>
    <version>1.2.1.Final</version>
  </dependency>
</dependencies>
````
