# Correcciones

**Integrantes:**
    - Samuel Moncada Salazar
    - Samuel Alejandro Ossa

## Error 1
- **Archivo:** app.py
- **Problema:** El puerto estaba en 5001 en vez de 5000
- **Solución:** Cambie `port=5001` por `port=5000`

## Error 2
- **Archivo** test_app.py
- **Problema:** la funcion `test_health` intenta encontrar la clave `uptime_seconds` pero la funcion health la devuelve dentro del json
- **Solución:** Cree la variable `uptime_seconds`, se le asgina un valor, y se devuelve dentro del json.

## Error 3
- **Archivo:** test_app.py
- **Problema:** La funcon metrics tenia la ruta `metrics` en vez de `metric`
- **Solución:** Cambie `metrics` por `metric`

## Error 4
- **Archivo:** docker-compose.yml
- **Problema:** El puerto del servicios `api` estaba en 5001 en vez de 5000
- **Solución:** Cambie `5000:5001` por `5000:5000`

## Error 5
- **Archivo:** requirements.txt
- **Problema:** El archivo no estaba completo
- **Solución:** Corrí el comando pip freeze > requirements.txt