---------------Espanish----------
Inicialización y configuración de Pygame: La primera parte del código importa el módulo pygame y realiza la configuración inicial necesaria, como establecer el tamaño de la ventana del juego.

Clases de los sprites: Se definen las clases principales utilizando la funcionalidad de sprites de Pygame: Player,Meteor, Bullet, Explosion. Estas clases heredan de la clase pygame.sprite.Sprite. Cada clase tiene métodos como update() para actualizar la posición de los sprites y manejar las colisiones.

Grupos de sprites: Se crean los grupos de sprites utilizando pygame.sprite.Group(). Los grupos se utilizan para actualizar y dibujar los sprites correspondientes.

El juego cuenta con una variedad de animaciones y sonidos para mejorar la experiencia del usuario. Cabe resaltar que se cuentas con funciones de disparos y un sistema de vida para saber el daño que se te haga en el juego.

Bucle principal del juego: El bucle while running es el núcleo del juego. Maneja los eventos del teclado, actualiza la posición de los sprites, maneja las colisiones y realiza el renderizado de la pantalla.

Control de velocidad de actualización: El reloj (clock) se utiliza para controlar la velocidad de actualización de la pantalla. En este caso, se establece en 60 actualizaciones por segundo.

Renderizado de la pantalla: Dentro del bucle principal, se dibuja la pantalla con screen.fill() para pintarla de negro, y luego se dibujan todos los sprites en all_sprites.draw(screen).

Colisiones: El código maneja las colisiones entre las balas y los enemigos utilizando pygame.sprite.groupcollide(). Si una bala colisiona con un enemigo, se eliminan ambos y se crea un nuevo enemigo.

Control de finalización del juego: Si el jugador colisiona con un enemigo, la variable running se establece en False, lo que detiene el bucle principal y finaliza el juego.

Cierre de Pygame: Una vez que el bucle principal se ha detenido, se llama a pygame.quit() para cerrar la ventana y finalizar el programa.

----------------------------English-------------------------------------------
Pygame initialization and configuration: The first part of the code imports the pygame module and does the necessary initial configuration, such as setting the size of the game window.

Sprite classes: The main classes are defined using the sprite functionality of Pygame: Player, Meteor, Bullet, Explosion. These classes inherit from the pygame.sprite.Sprite class. Each class has methods like update() to update the sprite position and handle collisions.

Sprite groups: The sprite groups are created using pygame.sprite.Group(). The groups are used to update and draw the corresponding sprites.

The game features a variety of animations and sounds to enhance the user experience. It should be noted that you have shooting functions and a life system to know the damage that is done to you in the game.

Main Game Loop: The while running loop is the core of the game. Handles keyboard events, updates sprite position, handles collisions, and performs screen rendering.

Refresh Rate Control: The clock is used to control the refresh rate of the screen. In this case, it is set to 60 updates per second.

Screen rendering: Inside the main loop, the screen is drawn with screen.fill() to paint it black, and then all sprites are drawn in all_sprites.draw(screen).

Collisions: The code handles collisions between bullets and enemies using pygame.sprite.groupcollide(). If a bullet collides with an enemy, both are removed and a new enemy is created.

Game Over Check: If the player collides with an enemy, the running variable is set to False, which stops the main loop and ends the game.

Pygame Quit: Once the main loop has stopped, pygame.quit() is called to close the window and end the program.