<div align="center">

# José Miguel Tirado Quiroz

**Security & Infrastructure Engineer** · Lima, Perú

<sub>Verificación formal · Redes empresariales · Automatización · Sistemas distribuidos</sub>

</div>

---

## Qué hago

Diseño y construyo sistemas que otros no tienen que operar a ciegas: infraestructura de red
empresarial, plataformas de orquestación multi-agente con **garantías formales de corrección**,
y capas de seguridad que se sostienen **a nivel de base de datos**, no solo en la aplicación.

Mi formación formal es en redes y telecomunicaciones. **Todo lo demás es autodidacta** — y en
seguridad, desde los 14 años.

---

## Repos destacados

<table>
<tr>
<td width="50%" valign="top">

### <a href="https://github.com/ElechugasCheraxxx/Cheraxxx-RedTeam-IDE">Cheraxxx RedTeam IDE</a>

**Orquestación multi-agente con verificación formal**

Plataforma de security assessment donde la máquina de estados del engagement está
especificada en **Coq 8.20 e Isabelle/HOL 2024** — es *matemáticamente imposible* saltar a
una fase ofensiva sin completar las fases de autorización previas.

Arquitectura políglota de 10+ lenguajes:

| Capa | Tecnología |
|---|---|
| Core | C++23 · Metal MPS (Apple Silicon) |
| Criptografía | Rust · ML-KEM-768 (FIPS 203) · ML-DSA-65 (FIPS 204) |
| Orquestación | Go + gRPC · Perl · Ruby (mruby) · Bun/TypeScript |
| Payloads | Zig |
| Protección | C / ASM · KEXT (macOS) · KMDF (Windows) |
| Verificación | Coq · Isabelle/HOL · *dual-path execution* |

<sub>[[code](https://github.com/ElechugasCheraxxx/Cheraxxx-RedTeam-IDE)]</sub>

</td>
<td width="50%" valign="top">

### <a href="https://github.com/ElechugasCheraxxx/LeadLayer-Compliance">LeadLayer Compliance</a>

**Seguridad y protección de datos a nivel de BD**

Referencia de ingeniería para SaaS B2B bajo la **Ley 29733** (Perú). La mayoría del
compliance se implementa en la aplicación — y falla en cuanto alguien escribe un `SELECT`
crudo. Aquí se baja al stack:

- **Log de consentimiento inmutable** con reglas Postgres (`CREATE RULE ... DO INSTEAD NOTHING`)
- **Row Level Security** para aislamiento multi-tenant que sobrevive a inyecciones SQL
- **Índices parciales** que cierran oráculos de temporización en el hot path de supresión
- **Auditor de cadena de suministro**: detecta resoluciones desde refs git, ausencia de hash
  de integridad y registries no oficiales
- **11 auditorías de seguridad** documentadas · pre/postcondiciones con property-based testing
- Procedimiento de registro ante el **RNPDP** (Art. 27, Ley 29733)

<sub>[[code](https://github.com/ElechugasCheraxxx/LeadLayer-Compliance)]</sub>

</td>
</tr>
<tr>
<td width="50%" valign="top">

### <a href="https://github.com/ElechugasCheraxxx/SDPipeline">SDPipeline</a>

**App nativa macOS · 53.000+ líneas de Swift**

Front-end de escritorio para Stable Diffusion sobre Apple Silicon.

- **28 motores de pipeline**: ControlNet, IP-Adapter, IC-Light, ADetailer, upscaling por
  teselas, composición de escenas
- **20 gestores** de ciclo de vida de modelos, trabajos y backups
- **Metal Performance Shaders** afinados para memoria unificada
- Búsqueda semántica de assets con **embeddings CLIP**
- Versionado de assets con historial completo · `IntegrityManager` · `AppHardeningManager`

<sub>[[code](https://github.com/ElechugasCheraxxx/SDPipeline)]</sub>

</td>
<td width="50%" valign="top">

### PRAECCE

**Motor de autocorrección distribuida** *(privado — disponible bajo acuerdo)*

Motor de corrección de errores autónoma con consenso por **quórum tipo Raft** y verificación
formal replicada en **Coq, Isabelle/HOL e Isabelle/ML**.

- Cadena de recuperación en tres etapas con pruebas de **caos por failpoint**:
  caída total de nodos, corrupción de blackboard, corrupción de memoria
- Buffer de auditoría *lock-free* sobre memoria compartida
- `rdtsc` en ensamblador x86_64/arm64 para precisión sub-nanosegundo

<sub>Contacto para más detalles</sub>

</td>
</tr>
</table>

---

## Stack

<table>
<tr><td valign="top" width="50%">

**Infraestructura &amp; Redes**
<br>TCP/IP · VLANs · STP · OSPF · BGP · VPN (IPsec/SSL) · SD-WAN · QoS · MPLS · E1/T1
<br>Cisco IOS · controladores wireless · PBX/VoIP · análisis OSI · packet sniffing

**Windows Server &amp; Linux**
<br>Active Directory · Group Policy · FSMO · DHCP/DNS/WDS · DFS Replication · Office 365
<br>RHEL/CentOS · Ubuntu Server · systemd · shell scripting

**Virtualización &amp; Nube**
<br>VMware vSphere/ESXi · Nutanix AHV · Hyper-V · Terraform (módulos VPC/RDS/Redis/S3)

</td><td valign="top" width="50%">

**Seguridad**
<br>Pentesting autorizado · reversing y análisis binario · OWASP · ISO 27001
<br>IPS/IDS · Anti-DDoS · hardening de endpoints · criptografía post-cuántica
<br>Row Level Security · supply-chain security · compliance Ley 29733

**Desarrollo &amp; Sistemas**
<br>Rust · C++23 · Go · Swift/SwiftUI · Zig · Ruby · Perl · TypeScript · Objective-C
<br>Metal/MPS · Coq · Isabelle/HOL · ensamblador x86_64/arm64
<br>Python · PowerShell · Git · CI/CD · infraestructura como código

</td></tr>
</table>

---

## Experiencia

| Periodo | Rol | Empresa |
|---|---|---|
| **Jul 2025 – Presente** | Consultor Independiente — Ciberseguridad e Ingeniería de Sistemas | Freelance |
| May – Jul 2025 | Analista de Infraestructura y Redes | Stefanini Sapia Group S.A.C. |
| Feb – May 2025 | Analista de Soporte Técnico L2/L3 | EMPETEC S.A.C. |
| Ene 2021 – Dic 2024 | Técnico en Infraestructura y Redes de Telecomunicaciones | Totonet S.A.C. |

---

## Certificaciones

**Cisco Networking Academy — CCNA v7 (×4)**

- Enterprise Networking, Security, and Automation (2024)
- Introduction to Networks (2024)
- Introduction to Cybersecurity (2023)
- Cybersecurity Essentials (2023)

**En curso:** Técnico en Administración de Redes y Comunicaciones — CIBERTEC

---

## Contacto

<sub>Disponible inmediatamente para Lima (presencial/híbrido) y remoto en LatAm.</sub>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/josé-miguel-tirado-quiroz)
[![Email](https://img.shields.io/badge/Email-jhoshuastevens556@icloud.com-2B6CB0?style=flat-square&logo=gmail&logoColor=white)](mailto:jhoshuastevens556@icloud.com)

---

<div align="center">
<sub>Hecho en Lima, Perú ☕</sub>
</div>
