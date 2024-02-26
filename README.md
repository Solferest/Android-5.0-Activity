# Android-5.0-Activity
# Логи при запуске приложения:
2024-02-26 13:42:01.931 14670-14670 MainActivityLog         com.example.myapplication2           D  CREATE log hello  
2024-02-26 13:42:02.057 14670-14670 MainActivityLog         com.example.myapplication2           D  START log hello  
2024-02-26 13:42:02.062 14670-14670 MainActivityLog         com.example.myapplication2           D  RESUME log hello  
  
onCreate() - создание приложения, подготовка к отображению  
OnStart() -  отображение приложения для пользователя  
OnResume() - пользователь может взаимодействовать с приложением, это состояние сохраняется, пока не произойдут какие-то события  

# Логи при повороте экрана:
2024-02-26 13:43:59.073 14670-14670 MainActivityLog         com.example.myapplication2           D  PAUSE log hello  
2024-02-26 13:43:59.080 14670-14670 MainActivityLog         com.example.myapplication2           D  STOP log hello  
2024-02-26 13:43:59.124 14670-14670 MainActivityLog         com.example.myapplication2           D  DESTROY log hello  
2024-02-26 13:43:59.206 14670-14670 MainActivityLog         com.example.myapplication2           D  CREATE log hello  
2024-02-26 13:43:59.215 14670-14670 MainActivityLog         com.example.myapplication2           D  START log hello  
2024-02-26 13:43:59.233 14670-14670 MainActivityLog         com.example.myapplication2           D  RESUME log hello  
  
onPause() - пользователь покидает приложение, но оно еще остается видимым  
onStop() - приложение перестает быть видимым  
onDestroy() - приложение временно уничтожается, чтобы потом отобразиться в состоянии поворота экрана  
onCreate() - создание приложения, подготовка к отображению  
OnStart() -  отображение приложения для пользователя  
OnResume() - пользователь может взаимодействовать с приложением, это состояние сохраняется, пока не произойдут какие-то события  
  
# Логи при сворачивании приложения:
2024-02-26 13:45:37.968 14670-14670 MainActivityLog         com.example.myapplication2           D  PAUSE log hello  
2024-02-26 13:45:38.587 14670-14670 MainActivityLog         com.example.myapplication2           D  STOP log hello  
  
onPause() - пользователь покидает приложение, но оно еще остается видимым  
onStop() - приложение перестает быть видимым  

# Логи при разворачивании:
2024-02-26 13:46:39.615 14670-14670 MainActivityLog         com.example.myapplication2           D  START log hello  
2024-02-26 13:46:39.617 14670-14670 MainActivityLog         com.example.myapplication2           D  RESUME log hello  
  
OnStart() -  отображение приложения для пользователя  
OnResume() - пользователь может взаимодействовать с приложением, это состояние сохраняется, пока не произойдут какие-то события  
Вызова onCreate() не происходит, поскольку приложение не было уничтожено  
  
# Логи при вызове метода finish():
2024-02-26 13:48:30.669 14919-14919 MainActivityLog         com.example.myapplication2           D  CREATE log hello  
2024-02-26 13:48:31.841 14919-14919 MainActivityLog         com.example.myapplication2           D  DESTROY log hello  
  
onCreate() - создание приложения  
onDestroy() - уничтожение приложения  
Так как вызов finish() происходит сразу после запуска onCreate(), приложение не успевает отобразиться для пользователя  
