# Plantilla de Palbin.com para el modo de consentimiento (Consent Mode) en GTM
Plantilla de Palbin.com para el modo de consentimiento en Google Tag Manager

## Creación de tags basados en la plantilla
Usa esta plantilla como base para generar 2 tags en tu GTM. Antes de generar los tags, asegúrate de tener configuradas todas las variables de capa de datos necesarias.

### Un tag para el modo de consentimiento por defecto
Este tag debe lanzarse con el activador "Consent Initialization - All Pages"

### Un tag para la actualización del modo de consentimiento
Este tag debe lanzarse con el activador `{{palbin.trigger.consentmode.update}}` que se lanzará cuando el usuario acepte o deniege el uso de cookies en el banner de cookies avanzadas.
Este tag debe establecer los parámetros del consentimiento utilizando las siguientes "variables de capa de datos" que Palbin.com pone a disposición:
- `{{palbin.consentmode.modes.ad_personalization}}`
- `{{palbin.consentmode.modes.ad_storage}}`
- `{{palbin.consentmode.modes.ad_user_data}}`
- `{{palbin.consentmode.modes.analytics_storage}}`
- `{{palbin.consentmode.modes.functionality_storage}}`
- `{{palbin.consentmode.modes.personalization_storage}}`
- `{{palbin.consentmode.modes.security_storage}}`
