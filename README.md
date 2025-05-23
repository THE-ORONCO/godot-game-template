# *Your game here*

Download Godot Here: https://godotengine.org/download

## godot-game-template

A minimal template for Godot games. Works with 2D and 3D games.

## Features

### Single- und Multilevel Betrieb
Das Template kann über Einstellungen in `Gamemanager` entweder ein einzelnes oder eine Folge von Levels laden. Dabei ist es egal, ob es 2D oder 3D Levels sind, solange sie über ein `win()`-Signal Bescheid geben, wann sie vervollständigt wurden. Wenn man eine Folge an Levels verwendet (wie in Super Mario) können diese hintereinander geladen werden, solange sie eine einheitliche Namenskonvention mit aufsteigenden Levelzahlen haben. Zum Beispiel `level_1.tscn`, `level_2.tscn`, ...

### Settings und Input Remapping
Mithilfe des `Settings`-Autoloads können einfach neue Einstellungen hinzugefügt werden (siehe Setting-Klasse), pro Setting kann ein Callback definiert werden, welches eine Änderung der entsprechenden Einstellung behandelt (z.B. Grafikvoreinstellung geändert -> Update alle Viewports). Das Settings-System hat auch eingebaute Unterstützung für Input-Remapping (2 Slots pro Action). Das Template kommt mit einem Einstellungsmenü, worüber die Zuweisung während der Laufzeit dynamisch geändert werden kann; dabei werden alle Inputs unterstützt, die Godot kennt. Häufig benötigte Einstellungen wie Vollbild-Modus, Lautstärke, etc. sind bereits vorhanden

### Umfangreicher Credit Screen
Die Inhalte des Credit-Screens werden aus `credits.json` eingelesen. Dort kann Name, Beschreibung, Lizenz und URL eines Assets angegeben werden. Standardmäßig sorgt der Credit Screen nicht nur dafür, dass die MIT Lizenz dieses Templates von darauf basierenden eingehalten wird, sondern er erfüllt (nach bestem Wissen) auch die Bedingungen zum crediten von Godot selbst.

### Optionale Tests inklusive GitHub Action
Im `with-tests`-Branch ist GdUnit4 aufgesetzt inclusive eines kleinen Tests, der testet, ob der zentrale Gamemanager gestartet werden kann. Zusätzlich enthält dieser Branch auch eine bereits aufgesetzte GitHub Action, die alle Tests mit jedem Commit ausführt. So wird es schnell ersichtlich, ob die aktuellste Version des Spiels überhaupt ausführbar ist.

### Ingame Debug Panel
Um wichtige Werte immer im Augenwinkel zu haben verfügt das Template über eine Debug Anzeige in der linken oberen Ecke. Über das `DebugGlobal`können Werte zur Debug Anzeige hinzugefügt werden. Die Sichtbarkeit kann über die, in der InputMap bereits definierten, `toggle_debug_label`-Action getoggelt werden.

### Spiel pausieren
Wenn die `pause`-Action der InputMap in einem Level ausgeführt wird, wird ein Pausemenü angezeigt, indem das Level beendet, -fortgeführt, oder Einstellungen angepasst werden. Wenn der `ProcessMode` der Levels auf "Pausable" gesetzt ist, werden die Aktivitäten im Level mitpausiert, solange das Pausemanü angezeigt wird.


## Further reading
### Tutorials
#### GDquest
https://www.youtube.com/@Gdquest

#### Brackeys
https://www.youtube.com/@Brackeys

#### Docs
https://docs.godotengine.org/en/latest/

#### Pixel Art
https://saint11.art/blog/pixel-art-tutorials/

#### Sakurai (Game Design)
https://www.youtube.com/@sora_sakurai_en 

### Tools
#### Aseprite (Pixelart)
> kostet etwas, wer es aber selbst compiliert bekommt kann es kostenlos nutzen (https://github.com/aseprite/aseprite/)
https://www.aseprite.org/ 

#### graphicsGale (Pixelart)
https://graphicsgale.com/us/

#### Audacity (Audio)
https://www.audacityteam.org/download/

#### Krita (2D-Art)
https://krita.org/en/

#### Adobe Alternatives
https://github.com/KenneyNL/Adobe-Alternatives

#### TrenchBroom (Quake-Map Designer)
https://trenchbroom.github.io/

### Assets
Ein Sammlung an verschiedenen Websites mit kostenlosen Game-Assets: https://www.freegameassets.com/

> **IMMER AUF DIE LIZENZEN ACHTEN**

#### Kenney 🥰
https://www.kenney.nl/

#### Opengameart
https://opengameart.org/

#### Free Sound
https://freesound.org/

#### Sonisss
https://sonniss.com/gameaudiogdc/

#### Shaders
https://godotshaders.com/

### Templates
#### Karlsruhe

#### 3D Platformer
https://github.com/KenneyNL/Starter-Kit-3D-Platformer

#### FPS
https://github.com/KenneyNL/Starter-Kit-FPS

#### City-Builder
https://github.com/KenneyNL/Starter-Kit-City-Builder

#### Generic
https://github.com/KenneyNL/Starter-Kit-Basic-Scene

### Plugins

#### Aseprite Wizzard
https://github.com/viniciusgerevini/godot-aseprite-wizard

#### G.U.I.D.E (Input Manager)
https://github.com/godotneers/G.U.I.D.E

#### State Charts
https://github.com/derkork/godot-statecharts

#### GUT (Tests)
https://gut.readthedocs.io/en/9.3.1/

#### Ridiculous Coding
https://github.com/jotson/ridiculous_coding

#### Func_Godot (Quake Maps -> Godot)
https://github.com/func-godot

#### Debug Draw 3D
https://github.com/DmitriySalnikov/godot_debug_draw_3d

#### TODO Manager 
https://github.com/OrigamiDev-Pete/TODO_Manager

#### Edit Resources as Sheets
https://github.com/don-tnowe/godot-resources-as-sheets-plugin/

#### Limbo AI (Behavior Trees & State Machines)
https://github.com/limbonaut/limboai

#### Limbo Console (Dev-Konsole)
https://github.com/limbonaut/limbo_console

#### Godot Plushie
https://github.com/Robert-K/godot-plushie-viewport-pet

#### Phantom Camera
https://phantom-camera.dev/

#### Dialog Manager
https://github.com/nathanhoad/godot_dialogue_manager
