## Programación Orientada a Objetos

### Atributos
Son propiedades dentro de las clases que se usan para describir características particulares del objeto a definir.

#### Clase Alumno
| Nombre | Carrera | Semestre |
| ------ | ------- | -------- |
| ---    | ---     | ---      |
|        |         |          |
##### Métodos Constructores
- Observadores
- Modificadores
- Calculadores
- Especiales
- Auxiliares
### Métodos
- Método constructor
	- Sin parámetros
	- Con parámetros

### Herencia
Se usa para extender los atributos de una clase ya existente y crear una clase nueva con propiedades heredadas de la clase anterior.
### Clases
Son los objetos que se pueden construir y contienen atributos y métodos

```java
public class Libro {
	string titulo;
	string autor;
	
	public Libro(String elTitulo, String elAutor) {
		titulo = elTitulo;
		atuor = elAutor;
	}
	
	public void asginarAutor(String elAutor) {
		autor = elAutor;
	}
}
```

```java
public class AudioLibro extends Libro {
	int duracion;
}
```

Para mantener consistencia se recomienda manipular los atributos únicamente mediante los métodos modificadores y observadores

```java
public class Libro {
	private string titulo;
	private string autor;
	
	public Libro(String elTitulo, String elAutor) {
		titulo = elTitulo;
		atuor = elAutor;
	}
	
	public void asginarAutor(String elAutor) {
		autor = elAutor;
	}
}

public class AudioLibro extends Libro {
	public void asignarAutorDesconocido() {
		this.autor = "desconocido"; // ❌ 
	}
}

ejemplo = new Libro();
ejemplo.asignarAutorDesconocido();
```

```java
public class Libro {
	private string titulo;
	private string autor;
	
	public Libro(String elTitulo, String elAutor) {
		titulo = elTitulo;
		atuor = elAutor;
	}
	
	public void asginarAutor(String elAutor) {
		autor = elAutor;
	}
}

public class AudioLibro extends Libro {
	public void asignarAutorDesconocido() {
		this.asignarAutor("desconocido"); // ✅
	}
}

ejemplo = new Libro();
ejemplo.asignarAutorDesconocido();
```