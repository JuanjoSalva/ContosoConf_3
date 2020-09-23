# Module 3: Introduction to JavaScript

Wherever a path to a file starts with *[Repository Root]*, replace it with the absolute path to the folder in which the 20480 repository resides. For example, if you cloned or extracted the 20480 repository to **C:\Users\John Doe\Downloads\20480**, change the path: **[Repository Root]\AllFiles\20480C\Mod01** to **C:\Users\John Doe\Downloads\20480\AllFiles\20480C\Mod01**.

# Lab: Displaying Data and Handling Events by Using JavaScript

### Lab Setup

### Preparation Steps

Ensure that you have cloned the 20480C directory from GitHub (** https://github.com/MicrosoftLearning/20480-Programming-in-HTML5-with-JavaScript-and-CSS3/tree/master/Allfiles**). It contains the code segments for the labs and demos in this course.

### Exercise 1: Displaying Data Programmatically

#### Task 1: Review the existing code for the Schedule page

1.	Start Microsoft Visual Studio 2017.
2.	In Microsoft Visual Studio, on the **File** menu, point to **Open**, and then click **Project/Solution**.
3.	In the **Open Project** dialog box, browse to the **[Repository Root]\Allfiles\Mod03\Labfiles\Starter\Exercise 1** folder, click **ContosoConf.sln**, and then click **Open**.

>**Note**: If **Security Warning for ContosoConf** dialog box appears, clear **Ask me for every project in this solution** checkbox and then click **OK**.
>
>4.	In Solution Explorer, expand the **ContosoConf** project node, and then double-click **schedule.htm**.
>5.	Review the contents of the **schedule.htm** file and verify that the **schedule** page section contains the following markup:
>
>  ```html
>      <section class="page-section schedule">
>          <div class="container">
>              <h1>Schedule</h1>
>              <ul id="schedule"></ul>
>          </div>
>      </section>
>  ```
>
>6.	Verify that the file contains the following HTML markup towards the end:
>
>  ```html
>      <script src="/scripts/pages/schedule.js" type="text/javascript"></script>
>  ```
>
>7.	In Solution Explorer, expand the **scripts** folder.
>8.	Expand the **pages** sub-folder.
>9.	Double-click **schedule.js**.
>10.	Review the contents of the **schedule.js** file and verify that the first few lines contain the following code:
>
>  ```javascript
>      const schedule = [ 
>          {
>              "id": "session-1",
>              "title": "Registration",
>              "tracks": [1, 2]
>          },
>          {
>              "id": "session-2",
>              "title": "Moving the Web forward with HTML5",
>              "tracks": [1, 2]
>          },
>          {
>              "id": "session-3",
>              "title": "Diving in at the deep end with Canvas",
>              "tracks": [1]
>          },
>          {
>              "id": "session-4",
>              "title": "New Technologies in Enterprise",
>              "tracks": [2]
>          },
>          ...
>      ];
>  ```

#### Task 2: Write code to get the schedule list element on the Schedule page

1. In Solution Explorer, double-click **schedule.js**.

2. After the line containing the **TODO: Task 2** comment, add the following line of JavaScript:

   ```javascript
       const list = document.getElementById("schedule");
   ```

#### Task 3: Implement the createSessionElement function that creates the list item for a session

1. In **schedule.js**, after the line containing the **TODO: Task 3** comment, add the following JavaScript code:

   ```javascript
       const li = document.createElement("li");
       li.textContent = session.title;
       return li;
   ```

#### Task 4: Implement the displaySchedule function that adds session items to the list for display

1. In **schedule.js**, after the line containing the **TODO: Task 4** comment, add the following JavaScript code:

   ```javascript
       for (let i = 0; i < schedule.length; i++) {
           const li = createSessionElement(schedule[i]);
           list.appendChild(li);
       }
   ```

#### Task 5: Run the web application and view the Schedule page

1.	In Solution Explorer, double-click **schedule.htm**.
2.	On the **Debug** menu, click **Start Without Debugging**.
3.	In Microsoft Edge, if the message, "Intranet settings are turned off by default," appears, click **Don’t show this message again**.
4.	Verify that the list of sessions is displayed.
5.	Close Microsoft Edge.


>**Results**: After completing this exercise, you will have added the **Schedule** page, which displays the details of the conference sessions, to the ContosoConf application.

### Exercise 2: Handling Events

#### Task 1: Add check box HTML elements
## Laboratorio Módulo 3

Fichero de Instrucciones: Instructions\20480C_MOD03_LAK.md

Entregar el url de GitHub con la solución y un readme con las siguiente información:

1. **Nombres y apellidos:** Juan José Salvador Román
2. **Fecha:** 24/09/2020
3. **Resumen del Ejercicio:** 


4. **Dificultad o problemas presentados y como se resolvieron:** 
Pues creo que es correcto pero ya dudo porque tengo lio con los repositorios y no sé muy bien como saber que proyecto de un repositorio corresponde con qué proyecto de los recientes en el visual studio.

**NOTA**: Si no hay descripcion de problemas o dificultades, y al yo descargar el código para realizar la comprobacion y el código no funcionar, el resultado de la califaciación del laboratorio será afectado.



Fecha de entrega: Jueves 24 de septiembre de 2020

