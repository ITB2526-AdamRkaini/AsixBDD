# AsixBDD

## Cómo usar este proyecto

1. Inicia los contenedores:
   ```bash
docker-compose up -d
```

2. Abre phpMyAdmin en el navegador:
   ```
http://localhost:8081
```

3. Conéctate con:
   - usuario: `user`
   - contraseña: `password`

4. Importa el SQL en phpMyAdmin o desde la consola:
   ```bash
docker exec -i mysql_db mysql -uuser -ppassword < create.sql
```

## Archivos SQL disponibles

- `create.sql` — script de creación y datos iniciales
- `init_tech_summit.sql` — script alternativo ya guardado

## Notas

- La base de datos se guarda en el volumen Docker `db_data`.
- Si cierras y vuelves a abrir, solo necesitas ejecutar `docker-compose up -d` y luego usar phpMyAdmin.
