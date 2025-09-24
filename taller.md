//
// Created by ACER on 24/09/2025.
//

**Ejercicio_1**
classDiagram
Biblioteca  -->  Usuario
Biblioteca  -->  Libro
Biblioteca  -->  Prestamo
Usuario  -->  Prestamo
Libro  -->  Prestamo

    class Libro {
    +int idUnico
    +String titulo
    +String autor
    +String genero
    +String estado
    +prestar()
    +devolver()
    +mostrarInfo()
}

class Usuario {
+int numID
+String nombre
+consultarHistorial()
}

class Prestamo {
+int idPrestamo
+Date fechaInicio
+Date fechaDevolucion
+registrarPrestamo()
+registrarDevolucion()
}

class Biblioteca {
+List(Libro) listaLibros
+List(Usuario) listaUsuarios
+List(Prestamo) listaPrestamos
+mostrarLibrosDisponibles()
+mostrarLibrosPrestados()
}
}

**Ejercicio_2**
El diagrama UML mustra una clase Plato la cual debe tener un nombre (string) y su precio (float).
Esta clase esta relacionada en la propiedad list platos, que esta contenida en la clase Pedido.
Esto se relaciona en que para hacer un pedido se necesita tener la lista del los platos para el restaurante.
Pedido esta relacionado con la clase Cliente, para realizar el pedido se necesita los datos del Cliente,
el cual debe pedir el plato y generar su pedido.
