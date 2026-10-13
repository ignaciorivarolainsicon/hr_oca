# Módulos OCA para el pañol de InSiCon

Esta rama del fork de [OCA/hr](https://github.com/OCA/hr) conserva los módulos
seleccionados para desarrollar y probar el pañol de InSiCon en Odoo 19.

| Addon | Versión | Función |
| --- | --- | --- |
| [hr_personal_equipment_request](hr_personal_equipment_request/) | 19.0.1.0.0 | Solicitudes y asignaciones de equipamiento a empleados. |
| [hr_personal_equipment_stock](hr_personal_equipment_stock/) | 19.0.1.0.0 | Integración de las asignaciones con Inventario. |
| [hr_employee_ppe](hr_employee_ppe/) | 19.0.1.0.0 | Información, vencimientos y comprobantes de EPP. |

## Dependencias

Los módulos requieren los addons estándar `product`, `hr`, `mail`, `purchase`
y `stock`, además de las dependencias entre los tres módulos incluidos.
Sus manifiestos no declaran dependencias externas de Python.

`hr_personal_equipment_stock` tiene instalación automática cuando sus
dependencias están instaladas.

## Estado de la adaptación

El código proviene de Odoo 18. Los manifiestos se actualizaron a `19.0.1.0.0`
para permitir su evaluación en Odoo 19. La compatibilidad del código y los
circuitos funcionales todavía requieren adaptación y validación.

Se conservan las pruebas, traducciones, documentación y atribuciones originales
de cada addon para acompañar ese trabajo.

## Uso en el proyecto

El proyecto `odoo_sh_base` incorpora este fork como submódulo en `oca/hr`,
asociado a la rama `19.0_pañol`. Cada publicación del fork requiere actualizar
y publicar también la referencia del submódulo en el proyecto.

## Licencia y procedencia

Los tres módulos declaran licencia AGPL-3. Se conserva el archivo [LICENSE](LICENSE)
y los avisos de autoría originales. Los módulos proceden de la
[Odoo Community Association (OCA)](https://odoo-community.org/).
