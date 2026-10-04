# Política de datos del proyecto de presupuestos de obra

**Versión académica:** 4 de octubre de 2026. **Alcance:** datos y proveedores ficticios para este ejercicio.

## 1. Alcance
Esta política cubre la preparación de costos y presupuestos arquitectónicos con apoyo de IA, desde el primer contacto hasta la eliminación.
La persona responsable del expediente decide finalidades, accesos y plazos; el arquitecto valida los cálculos antes de entregar una propuesta.
Se tratan D1 (contacto), D2 (domicilio), D3 (planos vinculados), D4–D7 (partidas y costos disociados), conforme al inventario anexo.
No se prevé captar datos personales sensibles ni nómina individual. Si aparecieran, se detiene su incorporación y se reevalúa la base y el aviso.

## 2. Ciclo de vida
En **captura** se comunica el aviso, se documenta consentimiento o excepción aplicable y se solicita el mínimo de D1–D3.
En **almacenamiento**, D2 se cifra en tránsito y reposo en una nube contratada; la clave y los accesos por rol quedan separados y auditados.
En **uso**, el arquitecto trabaja con identificador de obra, verifica metrado y precios y registra correcciones de la salida de IA.
En **compartición**, el proveedor del modelo recibe solo D2g (zona general) y partidas D4–D7 sin nombres ni planos; no recibe D2 exacto.
En **retención** se revisa la finalidad al cierre; D2 se bloquea cuando deja de ser necesario y se conserva solo por el plazo legal o contractual pertinente.
En **eliminación** se suprime tras ese plazo de expediente y respaldos, se registra la operación y se comunica a terceros cuando proceda.

## 3. Normativa aplicable
La LFPDPPP mexicana vigente (texto con reforma del 14 de noviembre de 2025) guía licitud, consentimiento, finalidad, proporcionalidad y aviso (arts. 5–16).
También obliga a seguridad y confidencialidad (arts. 18 y 20), derechos ARCO y bloqueo/supresión (arts. 21–27), y reglas de transferencias (arts. 35–36).
El Reglamento (UE) 2024/1689 se usa como comparación: el caso descrito es un uso interno en México y no se ha acreditado ámbito UE ni clasificación de alto riesgo.
El NIST AI RMF 1.0 es orientación voluntaria para gobernar, mapear, medir y gestionar riesgos, no una ley.

## 4. Controles comprometidos
Mantener inventario D1–D7, aviso y registro de base de tratamiento; restringir D1–D3 por rol y registrar accesos.
Cifrar D2 en tránsito/reposo, separar llaves, respaldar con controles equivalentes y revisar bitácoras de acceso mensualmente.
Comparar una muestra de tres partidas con cotizaciones y mediciones externas; un arquitecto aprueba la versión final.
Evaluar proveedor nube y modelo, cláusulas de confidencialidad y borrado; registrar transferencias y verificar configuración sin entrenamiento.
Atender solicitudes ARCO, incidentes y cambios de finalidad; documentar bloqueo, plazos y supresión de respaldos.

## 5. Manejo de datos con herramientas de IA
Se envían instrucciones con partidas, cantidades y zona general D2g; nunca D1, D2 exacto, D3 ni nómina individual.
Antes de cada carga se ejecuta una lista de revisión de identificadores directos e indirectos, incluyendo combinaciones singulares.
Se usa una cuenta de trabajo aprobada con opciones de privacidad revisadas y un registro de fecha, finalidad y proveedor.
La respuesta generada se considera borrador: se contrastan precios, fuentes, cálculos y sesgos antes de su uso.

## 6. Revisión
El responsable revisará la política cada trimestre y cuando cambie el proveedor, el tipo de dato, el alcance o la ley.
Documentará fecha, cambio y responsable de la revisión, así como incidentes y solicitudes de titulares.
La primera aplicación operativa requerirá confirmar contratos, plazos de conservación y aviso específico del responsable real.
Esta versión describe un diseño de práctica con datos ficticios, no acredita cumplimiento efectivo de una empresa.

## Referencias
- Cámara de Diputados. (2025, reforma de 14 de noviembre). *Ley Federal de Protección de Datos Personales en Posesión de los Particulares*. https://www.diputados.gob.mx/LeyesBiblio/pdf/LFPDPPP.pdf
- Parlamento Europeo y Consejo. (2024). *Reglamento (UE) 2024/1689*. https://eur-lex.europa.eu/eli/reg/2024/1689/oj
- National Institute of Standards and Technology. (2023). *Artificial Intelligence Risk Management Framework (AI RMF 1.0)*. https://doi.org/10.6028/NIST.AI.100-1
