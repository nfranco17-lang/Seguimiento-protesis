```mermaid
graph TD
    %% Estilos de Nodos
    classDef central fill:#1f2937,stroke:#111827,color:#ffffff,font-weight:bold;
    classDef causa fill:#ecfdf5,stroke:#059669,color:#065f46;
    classDef causaInd fill:#f3f4f6,stroke:#4b5563,color:#1f2937;
    classDef efectoDir fill:#dcfce7,stroke:#16a34a,color:#14532d;
    classDef efectoInd fill:#f0fdf4,stroke:#22c55e,color:#166534;
    classDef cat fill:#15803d,stroke:#166534,color:#ffffff,font-weight:bold;

    %% Problema Central
    PC["<b>PROBLEMA CENTRAL</b><br/>Inadecuado seguimiento y registro de la evolución de pacientes con prótesis"]:::central

    %% --- CAUSAS (Parte Inferior) ---
    %% Categoría 1: Evaluación y Métricas
    CI1["<b>CAUSA INDIRECTA</b><br/>Procesos de ajuste largos e iterativos sin datos objetivos"]:::causaInd --> CD1["<b>CAUSA DIRECTA</b><br/>Falta de mecanismos de feedback directo sobre la prótesis"]:::causa
    CD1 --> PC

    %% Categoría 2: Registro del Paciente
    CI2["<b>CAUSA INDIRECTA</b><br/>Ausencia de herramientas fáciles para el auto-reporte diario"]:::causaInd --> CD2["<b>CAUSA DIRECTA</b><br/>Registro ineficaz de dolor, nivel de comodidad y frecuencia de uso"]:::causa
    CD2 --> PC

    %% Categoría 3: Gestión e Historial
    CI3["<b>CAUSA INDIRECTA</b><br/>Historial de seguimiento manual, fragmentado o disperso"]:::causaInd --> CD3["<b>CAUSA DIRECTA</b><br/>Dependencia exclusiva de citas presenciales muy espaciadas"]:::causa
    CD3 --> PC

    %% --- EFECTOS (Parte Superior) ---
    %% Eje 1: Diseño y Adaptación
    PC --> ED1["<b>EFECTO DIRECTO</b><br/>Mala adaptación progresiva del paciente a la prótesis"]:::efectoDir
    ED1 --> EI1["<b>EFECTO INDIRECTO</b><br/>Dificultad en la identificación temprana de complicaciones y molestias"]:::efectoInd
    EI1 --> CAT1["SEGUIMIENTO MÉDICO"]:::cat

    %% Eje 2: Uso y Comodidad
    PC --> ED2["<b>EFECTO DIRECTO</b><br/>Abandono del uso de la prótesis o falta de adherencia"]:::efectoDir
    ED2 --> EI2["<b>EFECTO INDIRECTO</b><br/>Pérdida de movilidad y disminución de la calidad de vida"]:::efectoInd
    EI2 --> CAT2["EVOLUCIÓN DEL PACIENTE"]:::cat

    %% Eje 3: Gestión Institucional
    PC --> ED3["<b>EFECTO DIRECTO</b><br/>Imposibilidad de realizar estudios de efectividad de dispositivos"]:::efectoDir
    ED3 --> EI3["<b>EFECTO INDIRECTO</b><br/>Aumento en la carga de atención por emergencias o revisiones tardías"]:::efectoInd
    EI3 --> CAT3["REGISTRO DE DATOS"]:::cat
