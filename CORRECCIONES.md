# Correcciones

**Integrantes:**
    - Samuel Moncada Salazar
    - Samuel Alejandro Ossa

## Error 1
- **Archivo:** app.py
- **Problema:** El puerto estaba en 5001 en vez de 5000
- **Solución:** Cambie `port=5001` por `port=5000`

## Error 2
- **Archivo:** app.py
- **Problema:** La funcon metrics tenia la ruta `metric` en vez de `metrics`
- **Solución:** Cambie `metric` por `metrics`

## Error 3
- **Archivo** test_app.py
- **Problema:** la funcion `test_health` intenta encontrar la clave `uptime_seconds` pero la funcion health la devuelve dentro del json
- **Solución:** Cree la variable `uptime_seconds`, se le asgina un valor, y se devuelve dentro del json.

## Error 4
- **Archivo:** docker-compose.yml
- **Problema:** El puerto del servicios `api` estaba en 5001 en vez de 5000
- **Solución:** Cambie `5000:5001` por `5000:5000`

## Error 5
- **Archivo:** requirements.txt
- **Problema:** El archivo no estaba completo
- **Solución:** Corrí el comando pip freeze > requirements.txt

## Error 6
- **Archivo:** Dockerfile
- **Problema:** La imagen python 3.11 es mas pesada
- **Solución:** Cambio `python:3.11` por `python:3.11-slim`

## Error 7
- **Archivo:** Dockerfile
- **Problema:** Solo se hacía COPY de appy.py --> limita la escalabilidad
- **Solución:** Cambie `COPY app.py .` por `COPY . .`

## Error 8
- **Archivo:** prometheus.yml
- **Problema:** En `metrics_path:` estaba la ruta `/metric`
- **Solución:** Cambie `metric` por `metrics`