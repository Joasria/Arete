# Arete
Arete és un asistent virtual amb funcions de IA, la seva major diferència i virtud és ser un usuari virtual, pot realitzar i apendre feines i processos com si fos una persona de carn i ossos.

# Estructura
La estructura d'Arete, és totalment modular i aquests moduls és poden utilitzar de manera sincrònica o asincrònica i en l'ordre convenient per al workflow seleccionat que és on resideix la "inteligència" de l'asistent. Es tracta de generar "Raids" per a obtenir resultats.

-Main.py: La seva funció és la d'arrancar i sentar consideracions previes o fer ajustos de baix nivell en el programa.
  - verificació de l'estructura i creació d'ella si no existeix
  - verificació de les variables (pipe,
  - inicialització de la finestra principal
  - sortir

-Finestra.py: S'encarrega de les operatives de les diferents finestres, posició, tamany i mòdul de contingut, aixi com de monitoritzar la pipe per a eliminar-les, amagar-les, mostrar-les...
  - Genera la finestra principal
  - Genera el esquema de posicionament
  - Monitoritza la pipe
  - Obra i posiciona noves finestres.
  - Mostra o amaga finestres existents.
  - Tanca finestres amb processos acabats.

-Moduls de finestra (F*.py): són els pensats per a executar-se dins d'una finestra que mostrarà diferents opcions o informació sobre el procés.
  Exemples:
  - Finestra principal.
  - Finestra de chat.
  - Per a visualitzar camares.
  - ...

-Moduls de codi (M*.py): són aquells destinats a realitzar petites funcions a través d'un
