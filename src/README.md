# Kata TODO

```Gherkin
Feature: Gestión de Lista de Tareas

  Background: Al Iniciar la Aplicación

      Scenario: La Lista de Tareas debe estar vacía
      Given que el usuario ha iniciado la aplicación
      Then la lista de tareas debe estar vacía
      And la entrada de tareas debe estar vacía

  Background: Agregar Tareas a la Lista

      Scenario: Agregar Tarea con Contenido Válido
      Given que el usuario ha ingresado una tarea válida
      When hace clic en el botón "Add"
      Then el contenido de la entrada debe aparecer en el listado de tareas
      And la entrada de tareas debe estar vacía

      Scenario: Longitud del Nombre de la Tarea
      Given que el usuario ha ingresado una tarea con un nombre de más de 100 caracteres
      When hace clic en el botón "Add"
      Then se debe mostrar un mensaje de error y la tarea no debe ser agregada al listado

  Background: Marcar y Eliminar Tareas

      Scenario: Marcar Tarea como Completada
      Given que el usuario hace clic en una tarea
      When la tarea se marca como completada
      Then la tarea debe aparecer con estilo tachado en el listado de tareas

      Scenario: Eliminar Tarea al Hacer Clic en Botón "X"
      Given que el usuario hace clic en el botón "X" de una tarea
      When confirma la eliminación
      Then la tarea debe ser removida del listado de tareas
```
