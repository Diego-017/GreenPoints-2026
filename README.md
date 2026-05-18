# GreenPoints — Laravel Computo 3 C3

UNIVERSIDAD GERARDO BARRIOS

Materia: Programación Computacional IV

Docente: Willian Alexis Montes Girón

Integrantes

Diego Martín López Moreno (SMSS097824).  

Walter Alexander Ramírez Benítez (SMSS082124).  

Juan Ramón Espinal Coto (SMSS102323).  

Franklin Aldahir Portillo Flores (SMSS011624).  

Omar Salvador García Vasquez (SMSS093524).  

Flor Marina Torres Jandres (SMSS098424).  

Grupo: B2

Fecha: 17 mayo  2026.

## Estructura implementada

### Modelos (app/Models/)
| Modelo | Tabla | Descripción |
|---|---|---|
| Role | roles | Roles del sistema (admin, usuario) |
| User | users | Usuarios con puntos y rol |
| AccionEcologica | acciones_ecologicas | Tipos de reciclaje con puntos |
| RegistroAccion | registros_acciones | Historial de reciclajes por usuario |
| Dispositivo | dispositivos | Puntos ecológicos físicos |
| Premio | premios | Catálogo de premios canjeables |
| Canje | canjes | Historial de canjes realizados |

### Controladores y rutas
| Módulo | Rutas implementadas |
|---|---|
| Auth | GET/POST login, register — POST logout |
| Dashboard | GET /dashboard |
| Reciclaje | GET index, GET create, POST store, DELETE destroy |
| Premios | GET index, POST canjear |
| Dispositivos | GET index, GET create, POST store, GET edit, PUT update, DELETE destroy |

### Vistas (resources/views/)
- `landing.blade.php` — Página pública de inicio
- `auth/login.blade.php` — Login
- `auth/register.blade.php` — Registro
- `layouts/app.blade.php` — Layout principal con sidebar
- `dashboard/index.blade.php` — Panel del usuario
- `reciclaje/index.blade.php` — Lista de reciclajes
- `reciclaje/create.blade.php` — Formulario de registro
- `premios/index.blade.php` — Catálogo + canje + historial
- `dispositivos/index.blade.php` — Lista de dispositivos
- `dispositivos/create.blade.php` — Registrar dispositivo
- `dispositivos/edit.blade.php` — Editar dispositivo

---

## Módulos pendientes para siguiente avance

- Panel de administración (estadísticas globales, gestión de usuarios)
- Gestión de acciones ecológicas desde el panel admin
- Subida de imágenes para premios y dispositivos
- Sistema de roles y middleware para restringir acceso admin
- Notificaciones y correos
