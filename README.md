# Lista de comandos para react-native

```
//Crear aplicación utilizando expo
npx create-expo-app@latest nombre-app --template blank

//Iniciar ejecución de aplicación expo
npx expo start

//Instalar todas las librerías definidas en el package.json
npm install

//Instalar librería para guardar en almacenamiento datos
npm install @react-native-async-storage/async-storage

//Instalar librerías para navegar en una aplicación react
npm i @react-navigation/native
npm i @react-navigation/drawer
npm i @react-navigation/bottom-tabs
npm i @react-navigation/stack

//Instalar librerías de complemento para las librerías de navegación
npm i react-native-gesture-handler
npm i react-native-reanimated
npm i react-native-screens
npm i react-native-safe-area-context 
npx expo install react-native-reanimated

//Instalar librería para personalizar la status-bar
npm i expo-status-bar

//Instalar librería para crear gráficos
npm i react-native-chart-kit

//Instalar librería para utilizar iconos en aplicación
npm i react-native-vector-icons

npm i react-id-generator
npm i react-native-svg
```

## Construir apk con expo
```
npm install -g eas-cli
eas login
eas whoami
eas build:configure

eas build -p android --profile preview
```

### Formato de eas.json
```
{
  "cli": {
    "version": ">= 10.2.2"
  },
  "build": {
    "development": {
      "developmentClient": true,
      "distribution": "internal"
    },
    "preview": {
      "android": {
        "buildType": "apk"
      }
    },
    "production": {}
  },
  "submit": {
    "production": {}
  }
}
```

