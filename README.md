# CustomTitlebar

CustomTitlebar is a project where the main class (QCustomWindow) inherits its properties from QMainWindow, part of Qt Library.
Inheriting the main window from the QCustomWindow class, will allow you to develop programs which will use customized borders (not generated by the OS) - have a look at the screenshots for major details.																						

<p align="center">
  <img src="/Screenshots/winNormal.png">
</p>

## Support and Documentation

Docs elaboration is still in progress :( ...
Should you have any doubts, do not hesitate in contacting me through [my email](mailto:mauro.mascarenhas@nintersoft.com).

## Features:

- Customized stylesheet (light theme);
- Resizeable (100% functional);
- Window title update (QMainWindow::setWindowTitle(QString)) working properly;
- Better performance (when compared to previous versions);
- QTabWidgets and QDockWidgets working properly;
- QMenuBar/menu widget can be through QCustomWindow methods (DO NOT CALL IT THROUGH ITS PARENT (QMAINWINDOW) METHODS);
- Available as a Dynamically Linked Library (DLL).

## Limitations:

- It is not recommended to change QToolBar's stylesheet (after it has been added to the QCustomWindow's layout), since the auto-generated one plays and important role in the layout disposition;
- Setting the menu bar/widget through QMainWindow's methods will possibly crash the application (so, it is not possible to generate it through Qt Designer). Should you do that, the window's titlebar is going to be removed and every reference to it is going to break (since the widget gets deleted);

## Distribution (available versions):

-[X] DLL + LIB + headers;
-[X] Stactic linking/source files;
-[ ] Qt Creator/Designer plugin;

## CustomTitlebar open source code

- You can download and make modifications in the source code, accordingly to Mozilla Public Licence v2.0 terms.
- The licence is available in the root of the project folder and must be always shipped with it.