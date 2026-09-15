# Seguridad y privacidad

Mandarina procesa datos privados, incluidos movimientos financieros. Por eso la seguridad forma parte de la arquitectura:

- autenticación gestionada por Supabase Auth;
- Row Level Security para aislar los registros de cada usuario;
- operaciones sensibles ejecutadas en servidor;
- claves privadas fuera del navegador y del repositorio;
- validación de entradas en los límites del sistema;
- revisión de permisos tanto en la aplicación como en PostgreSQL.

Este repositorio es un caso de estudio. No contiene el código operativo, migraciones, backups, exportaciones ni información personal del sistema real.
