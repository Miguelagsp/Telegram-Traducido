## Telegram messenger para Android

[Telegram](https://telegram.org) es una aplicación de mensajería centrada en la velocidad y la seguridad. Es súper rápida, sencilla y gratuita.
Este repositorio contiene el código fuente oficial de [Aplicación de Telegram para Android](https://play.google.com/store/apps/details?id=org.telegram.messenger).

## Crear su aplicación de Telegram

Damos la bienvenida a todos los desarrolladores para que utilicen nuestra API y el código fuente para crear aplicaciones en nuestra plataforma.
Hay varias cosas que requerimos de **todos los desarrolladores** por el momento.

1. [**Obtener su propio api_id**](https://core.telegram.org/api/obtaining_api_id) for your application.
2. Por favor, **no** utilices el nombre de Telegram para tu aplicación - o asegúrate de que tus usuarios entienden que no es oficial.
3. Por favor, **no** utilice nuestro logotipo estándar (avión de papel blanco en un círculo azul) como logotipo de su aplicación.
3. Por favor, estudie nuestras [**directrices de seguridad**](https://core.telegram.org/mtproto/security_guidelines) y cuide bien los datos y la privacidad de sus usuarios.
4. Por favor, recuerda publicar también **tu** código para cumplir con las licencias.

### API, documentación del protocolo

Manuales de la API de Telegram: https://core.telegram.org/api

Manuales de protocolo MTproto: https://core.telegram.org/mtproto

### Guía de recopilación

**Nota**: Con el fin de apoyar [construcciones reproducibles](https://core.telegram.org/reproducible-builds), este repositorio contiene release.keystore, google-services.json y variables llenas dentro de BuildVars.java. Antes de publicar tus propios APKs, asegúrate de reemplazar todos estos archivos con los tuyos propios.

Necesitarás Android Studio 3.4, Android NDK rev. 20 y Android SDK 8.1

1. Descargue el código fuente de Telegram en https://github.com/DrKLO/Telegram ( git clone https://github.com/DrKLO/Telegram.git )
2. Copie su release.keystore en TMessagesProj/config
3. Rellene RELEASE_KEY_PASSWORD, RELEASE_KEY_ALIAS, RELEASE_STORE_PASSWORD en gradle.properties para acceder a su release.keystore
4.  Ve a https://console.firebase.google.com/, crea dos aplicaciones androides con los ID de aplicación org.telegram.messenger y org.telegram.messenger.beta, activa la mensajería de firebase y descarga google-services.json, que debe copiarse en la misma carpeta que TMessagesProj.
5. Abra el proyecto en el Estudio (tenga en cuenta que debe abrirse, NO importarse).
6. Rellena los valores en TMessagesProj/src/main/java/org/telegram/messenger/BuildVars.java - hay un enlace para cada una de las variables que muestra dónde y qué datos obtener.
7. Ya está listo para compilar Telegram.

### Localización

Hemos trasladado todas las traducciones a https://translations.telegram.org/en/android/. Por favor, utilícelo.

#### Traducido por Miguelagsp 
