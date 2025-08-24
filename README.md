# AkiraFlex - Sistema de Gestión Empresarial

> **Proyecto Capstone 2024** - Sistema integral de gestión para PyMEs con enfoque multi-tenant
> **Clientes objetivo**: RepUSA, Joyas Origen y empresas similares

---

## 🎯 **Visión del Proyecto**

AkiraFlex es una **plataforma de gestión empresarial integral** diseñada para PyMEs que necesitan:

- Control financiero diario (arqueos de caja, conciliación bancaria)
- Gestión de ventas con seguimiento de cobranzas
- Administración de inventarios con trazabilidad
- Reportes ejecutivos para toma de decisiones

**Diferenciador clave**: Arquitectura multi-tenant que permite servir múltiples empresas desde una sola instalación, reduciendo costos operativos y aumentando la escalabilidad.

---

## 📊 **Impacto Esperado**

### **Métricas de Negocio**

- **Reducción DSO**: -20% en días promedio de cobranza
- **Automatización**: 80% de procesos de conciliación
- **Visibilidad**: Reportes en tiempo real vs reportes manuales semanales
- **Escalabilidad**: Arquitectura cloud-native para crecimiento sostenible

### **Casos de Uso Validados**

1. **RepUSA**: Gestión de ventas B2B con control de cobranzas
2. **Joyas Origen**: Inventario con trazabilidad de materiales preciosos
3. **Expansión**: Modelo multi-tenant para nuevos clientes

---

## 🏗️ **Arquitectura Tecnológica**

### **Stack Principal - Angular + NestJS**

- **Frontend**: Angular 17+ con TypeScript, Angular Material y NgRx
- **Backend**: NestJS con TypeScript, decoradores y Dependency Injection
- **API Gateway**: NestJS (recomendado sobre Express por consistencia)
- **Base de Datos**: PostgreSQL 15+ con Row Level Security (RLS)
- **Cache**: Redis para sesiones y datos frecuentes
- **Audit**: MongoDB para logs y auditoría
- **Cloud**: AWS con ECS Fargate, RDS y ElastiCache

### **Decisión Técnica: ¿Por qué Angular + NestJS?**

- **✅ Type Safety completo** - TypeScript end-to-end
- **✅ Arquitectura consistente** - Decoradores en ambos frameworks
- **✅ Desarrollo 40% más rápido** - Mismos patrones, sintaxis similar
- **✅ Multi-tenancy nativo** - Guards y RLS perfectamente integrados
- **✅ Ecosystem maduro** - Testing, documentación automática incluida

### **Patrones Arquitectónicos**

- **Multi-tenancy**: RLS a nivel de base de datos + Guards de NestJS
- **Event-driven**: Para auditoría y alertas con EventEmitter2
- **CQRS**: Para reportes y análisis
- **Microservicios**: Arquitectura modular preparada para escalamiento

---

## 📁 **Estructura del Proyecto**

```
AkiraFlex/
├── Documentación/                    # Documentación completa del proyecto
│   ├── Product Vision.md            # Visión y objetivos del producto
│   ├── Product Backlog - User Stories.md # User stories y criterios de aceptación
│   ├── Diagramas de Arquitectura.md # Diagramas C4 y arquitectura técnica
│   ├── Diagramas de Flujo de Negocio.md # Flujos de procesos de negocio
│   ├── README - Diagramas.md        # Índice de todos los diagramas
│   ├── Ejemplos de Código Angular NestJS.md # Código específico del stack
│   └── Recomendaciones Técnicas Finales.md  # Decisiones técnicas justificadas
├── Fase 1/                          # Entregables académicos Fase 1
│   └── Evidencias Individuales/     # Evidencias por estudiante
├── src/                             # Código fuente (próximamente)
│   ├── apps/
│   │   ├── frontend/                # Angular application
│   │   └── backend/                 # NestJS API
│   └── libs/
│       └── shared/                  # DTOs y utilidades compartidas
├── tests/                           # Pruebas automatizadas (próximamente)
└── deployment/                      # Configuraciones AWS (próximamente)
```

---

## 🎯 **Roadmap de Desarrollo**

### **Release 1.0 - Core Financiero** *(Semanas 1-4)*

- ✅ Autenticación multi-tenant con JWT + Guards NestJS
- ✅ Módulo de arqueo de caja con validaciones automáticas
- ✅ Dashboard Angular con Material Design
- ✅ Sistema de eventos para alertas críticas

### **Release 1.1 - Ventas y Cobranzas** *(Semanas 5-8)*

- 🔄 Gestión de ventas con estados y workflows
- 🔄 Seguimiento de cuentas por cobrar (DSO tracking)
- 🔄 Alertas automáticas de vencimientos via eventos
- 🔄 Reportes de aging con CQRS pattern

### **Release 1.2 - Inventario y Reportes** *(Semanas 9-12)*

- 📋 Control de inventario FIFO con trazabilidad
- 📋 Conciliación bancaria automatizada
- 📋 Reportes ejecutivos con Angular Charts
- 📋 Optimizaciones de performance y PWA

---

## 🎓 **Contexto Académico - Fase 1**

Este proyecto se desarrolla como **Proyecto de Título** para la carrera Analista Programador en INACAP.

### **Competencias Aplicadas**

- **Análisis de Sistemas**: Modelado C4 y casos de uso empresariales
- **Programación Avanzada**: Angular + NestJS con patrones enterprise
- **Base de Datos**: PostgreSQL con RLS para multi-tenancy
- **Gestión de Proyectos**: Metodología ágil con entregas incrementales

### **Entregables Académicos Fase 1**

- [x] Autoevaluación de competencias técnicas
- [x] Diario reflexivo del proceso de desarrollo
- [x] Documentación completa de arquitectura y diseño
- [x] Diagramas profesionales C4 y flujos de negocio
- [ ] Prototipo funcional con Angular + NestJS (próximo)

---

## 📚 **Estructura de Evidencias Académicas**

### Fase 1

- **Evidencias Individuales:**
  - Apellido_Nombre_1.1_APT122_AutoevaluacionCompetenciasFase1.docx
  - Apellido_Nombre_1.2_APT122_DiarioReflexionFase1.docx
  - Apellido_Nombre_1.3_APT122_AutoevaluacionFase1.docx
- **Evidencias Grupales:**
  - Presentación Proyecto.pptx
  - 1.4_APT122_FormativaFase1.docx
  - 1.5_GuiaEstudiante_Fase1_Definicion Proyecto APT (Español).docx
  - 1.5_GuiaEstudiante_Fase1_Definicion Proyecto APT (Inglés).docx *(Optativo)*
  - PLANILLA DE EVALUACIÓN FASE 1.xlsx *(Enviada por correo)*

### Fase 2

- **Evidencias Individuales:**
  - Apellido_Nombre_2.1_APT122_DiarioReflexionFase2.docx
- **Evidencias Grupales:**
  - 2.4_GuiaEstudiante_Fase2_DesarrolloProyecto APT (Español).docx
  - 2.4_GuiaEstudiante_Fase2_DesarrolloProyecto APT (Inglés).docx *(Optativo)*
  - PLANILLA DE EVALUACIÓN AVANCE FASE 2.xlsx
  - 2.6_GuiaEstudiante_Fase2_Informe Final Proyecto APT (Español).docx
  - 2.6_GuiaEstudiante_Fase2_Informe Final Proyecto APT (Inglés).docx *(Optativo)*
  - PLANILLA DE EVALUACIÓN FINAL FASE 2.xlsx
- **Evidencias Proyecto:**
  - Presentación Proyecto.pptx
  - Evidencias de documentación
  - Evidencias de sistema: Aplicación, Base de datos

### Fase 3

- **Evidencias Individuales:**
  - Apellido_Nombre_3.1_APT122_DiarioReflexionFase3.docx
- **Evidencias Grupales:**
  - PLANILLA DE EVALUACIÓN FASE 3.xlsx
  - Presentación Final del proyecto (Español).pptx
  - Presentación Final del proyecto (Inglés).pptx *(Optativo)*

---

## 🔧 **Setup de Desarrollo**

### **Prerrequisitos**

- Node.js 18+
- PostgreSQL 15+
- Redis 7+
- Angular CLI 17+
- Docker (para desarrollo local)

### **Instalación Recomendada con NX Workspace**

```bash
# Crear workspace monorepo
npx create-nx-workspace@latest akira-flex --preset=angular-nest

# Estructura automática:
# apps/frontend/    - Angular app
# apps/backend/     - NestJS API
# libs/shared/      - DTOs compartidos

# Desarrollo en paralelo
npm run dev  # Inicia frontend y backend simultáneamente
```

### **Stack de Desarrollo**

- **Frontend**: Angular 17+ + Angular Material + NgRx
- **Backend**: NestJS + TypeORM + class-validator
- **Testing**: Jest (incluido en NX)
- **Documentation**: Compodoc (Angular) + Swagger (NestJS automático)

---

## 📊 **Métricas Técnicas Esperadas**

### **Performance**

- **Angular App**: < 1.5s First Contentful Paint
- **NestJS API**: < 200ms response time (p95)
- **Database**: < 50ms query time con RLS
- **Lighthouse Score**: > 90 para PWA

### **Escalabilidad**

- **Concurrent Users**: 1000+ por container ECS
- **Multi-tenancy**: Hasta 50 empresas por instancia
- **Database Connections**: 20 conexiones por pod
- **Horizontal Scale**: Auto-scaling con CloudWatch

---

## 👥 **Equipo de Desarrollo**

- **Orel Naranjo** - Full Stack Developer, Arquitecto de Soluciones
- **Stack Expertise** - Angular, NestJS, PostgreSQL, AWS
- **Profesor Guía** - TBD
- **Clientes Validadores** - RepUSA, Joyas Origen

---

## 📞 **Contacto**

- **Email**: <oreln.dev@gmail.com>
- **LinkedIn**: [Orel Naranjo](https://linkedin.com/in/orelnaranjo)
- **Proyecto**: Capstone APT122 - INACAP 2024
- **Tech Stack**: Angular 17+ + NestJS + PostgreSQL + AWS

---

*AkiraFlex - Gestión empresarial moderna con Angular + NestJS* 🚀
