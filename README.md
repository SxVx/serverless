Para los plugins consultados: https://github.com/serverless/plugins

plugins para el trabajo offline: https://github.com/dherault/serverless-offline

comandos:

crea un proyecto usando una platilla de nodejs, con el nombre curso-sls-hola-mundo
```bash
serverless create -t aws-nodejs -n curso-sls-hola-mundo
```

Elimina lo creado del serverless para que no deje rastro o evitar conflictos de actualización:
```bash
serverless remove
```

Invoca una función desde nuestra terminal por el nombre, -d es para pasar el input
```bash
serverless invoke -f api -d "Mi mensaje"
```

Hace deploy:
```bash
serverless deploy --verbose
```

Para configurar los accesos
( **Preferible usar:** aws configure )
```bash
serverless config credentials --provider aws --key <KEY_PUBLIC> --secret <KEY_SECRET>
```

Crea el acceso local:
```bash
sls offline
```

Tutorial para usar y crear diferentes perfiles para los proyectos:

https://youtu.be/fJwB027Bx8U?si=w5-D2XZyy6V-1gSE