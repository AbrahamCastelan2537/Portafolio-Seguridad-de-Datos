# Investigación: Conceptos Básicos de Seguridad de la Información

---

# 1️⃣ Triada CIA (Confidentiality, Integrity, Availability)


::contentReference[oaicite:0]{index=0}


La **Triada CIA** es el modelo fundamental de la seguridad de la información. Representa los tres pilares que deben protegerse en cualquier sistema tecnológico.

## Confidencialidad (Confidentiality)

Garantiza que la información solo sea accesible para usuarios autorizados.

**Mecanismos de protección:**
- Cifrado de datos (AES, TLS)
- Control de acceso basado en roles (RBAC)
- Autenticación fuerte
- Clasificación de información

**Ejemplo práctico:**  
Una base de datos médica protegida mediante cifrado y autenticación multifactor.

---

## Integridad (Integrity)

Asegura que la información no sea alterada sin autorización.

**Controles comunes:**
- Hashes criptográficos (SHA-256)
- Firmas digitales
- Logs auditables
- Control de versiones

**Ejemplo:**  
Un sistema bancario que verifica mediante hash que una transferencia no fue modificada.

---

## Disponibilidad (Availability)

Garantiza que los sistemas y datos estén accesibles cuando se necesiten.

**Medidas de protección:**
- Redundancia de servidores
- Backups periódicos
- Protección contra ataques DoS
- Sistemas UPS

**Ejemplo:**  
Un servidor con respaldo en la nube para evitar interrupciones.

---

# 2️⃣ Triángulo de Usabilidad (Usability Triangle)


::contentReference[oaicite:1]{index=1}


El Triángulo de Usabilidad representa el equilibrio entre:

- Seguridad  
- Usabilidad  
- Funcionalidad  

## Principio Fundamental

A mayor seguridad, puede disminuir la usabilidad.  
A mayor facilidad de uso, puede aumentar el riesgo.

**Ejemplo:**  
Contraseñas extremadamente complejas pueden generar malas prácticas como anotarlas en papel.

El objetivo es encontrar un equilibrio adecuado según el contexto organizacional.

---

# 3️⃣ Riesgo en Seguridad de la Información


::contentReference[oaicite:2]{index=2}


El **riesgo** es la probabilidad de que una amenaza explote una vulnerabilidad y genere un impacto negativo.

## Fórmula común

**Riesgo = Probabilidad × Impacto**

## Componentes del Riesgo

- Activo
- Amenaza
- Vulnerabilidad
- Impacto

## Clasificación del Riesgo

- Bajo
- Medio
- Alto
- Crítico

La gestión de riesgos implica identificar, analizar y mitigar riesgos mediante controles de seguridad.

---

# Autenticación Multifactor (MFA)


::contentReference[oaicite:3]{index=3}


La **Autenticación Multifactor (MFA)** requiere dos o más factores para verificar la identidad.

## Factores de Autenticación

1. Algo que sabes → contraseña  
2. Algo que tienes → token, celular  
3. Algo que eres → huella, reconocimiento facial  

## Beneficios

- Reduce robo de cuentas
- Mitiga ataques de fuerza bruta
- Protege contra phishing

La MFA fortalece principalmente la **confidencialidad** dentro de la Triada CIA.

---

# 5️⃣ Vulnerabilidad


::contentReference[oaicite:4]{index=4}


Una **vulnerabilidad** es una debilidad que puede ser explotada por una amenaza.

## Tipos de vulnerabilidades

- Técnicas (errores de programación)
- De configuración (puertos abiertos)
- Humanas (ingeniería social)
- Físicas (acceso no controlado)

La presencia de una vulnerabilidad incrementa el riesgo si existe una amenaza activa.

---

# 6️⃣ Amenaza


::contentReference[oaicite:5]{index=5}


Una **amenaza** es cualquier evento o actor con potencial de causar daño.

## Clasificación

- Naturales (incendios, terremotos)
- Técnicas (malware, DDoS)
- Humanas (hackers, insiders)

Las amenazas pueden ser intencionales o accidentales.

---

# 7️⃣ Impacto


::contentReference[oaicite:6]{index=6}


El **impacto** es la consecuencia negativa tras la explotación de una vulnerabilidad.

## Tipos de impacto

- Financiero
- Reputacional
- Operativo
- Legal
- Estratégico

**Ejemplo:**  
Un ataque ransomware puede paralizar operaciones y generar pérdidas económicas significativas.

---

# Relación entre Vulnerabilidad, Amenaza, Riesgo e Impacto

Un incidente ocurre cuando:

Vulnerabilidad + Amenaza = Explotación  
Explotación + Consecuencia = Impacto  
Probabilidad × Impacto = Riesgo  

Comprender esta relación permite priorizar controles de seguridad.

---

# Conclusión General

La seguridad de la información se basa en proteger la confidencialidad, integridad y disponibilidad de los datos. El análisis de riesgo permite evaluar la probabilidad y el impacto de posibles incidentes, mientras que mecanismos como la autenticación multifactor reducen significativamente la superficie de ataque.

La interacción entre vulnerabilidad, amenaza e impacto define el nivel de riesgo al que está expuesta una organización. Por ello, la seguridad no es un estado absoluto, sino un proceso continuo de mejora, evaluación y adaptación ante nuevas amenazas tecnológicas.