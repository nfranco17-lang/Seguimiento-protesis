```mermaid
graph BT
    %% Estilos de Nodos
    classDef central fill:#1f2937,stroke:#111827,color:#ffffff,font-weight:bold;
    classDef causa fill:#ecfdf5,stroke:#059669,color:#065f46;
    classDef causaInd fill:#f3f4f6,stroke:#4b5563,color:#1f2937;
    classDef efectoDir fill:#dcfce7,stroke:#16a34a,color:#14532d;
    classDef efectoInd fill:#f0fdf4,stroke:#22c55e,color:#166534;
    classDef cat fill:#15803d,stroke:#166534,color:#ffffff,font-weight:bold;

    %% --- PROBLEMA CENTRAL (Tronco) ---
    PC["PROBLEMA CENTRAL\nInadecuado seguimiento y registro de la evolución de pacientes con prótesis"]:::central

    %% ==========================================
    %% --- CAUSAS (Raíces - Parte Inferior) ---
    %% ==========================================

    %% Categoría 1: Evaluación y Métricas
    CI1["CAUSA INDIRECTA\nProcesos de ajuste largos e iterativos sin datos objetivos"]:::causaInd --> CD1["CAUSA DIRECTA\nFalta de mecanismos de feedback directo sobre la prótesis"]:::causa
    CD1 --> PC

    %% Categoría 2: Registro del Paciente
    CI2["CAUSA INDIRECTA\nAusencia de herramientas fáciles para el auto-reporte diario"]:::causaInd --> CD2["CAUSA DIRECTA\nRegistro ineficaz de dolor, nivel de comodidad y frecuencia de uso"]:::causa
    CD2 --> PC

    %% Categoría 3: Gestión e Historial
    CI3["CAUSA INDIRECTA\nHistorial de seguimiento manual, fragmentado o disperso"]:::causaInd --> CD3["CAUSA DIRECTA\nDependencia exclusiva de citas presenciales muy espaciadas"]:::causa
    CD3 --> PC

    %% Categoría 4: Comunicación Multidisciplinaria
    CI4["CAUSA INDIRECTA\nFalta de canales centralizados para compartir la historia clínica ortopédica"]:::causaInd --> CD4["CAUSA DIRECTA\nDescoordinación entre el equipo multidisciplinario (protesista, fisio, médico)"]:::causa
    CD4 --> PC
    %% Categoría 5: Tecnología y Monitoreo 
    CI5["CAUSA INDIRECTA\nBajo uso de dispositivos o sensores (wearables/IoT) que permitan captar datos objetivos entre citas"]:::causaInd --> CD5["CAUSA DIRECTA\nAusencia de tecnología de monitoreo remoto y continuo del estado del paciente"]:::causa
    CD5 --> PC

    %% Categoría 5: Tecnología y Monitoreo
    CI5["CAUSA INDIRECTA\nBajo uso de dispositivos o sensores (wearables/IoT) que permitan captar datos objetivos entre citas"]:::causaInd --> CD5["CAUSA DIRECTA\nAusencia de tecnología de monitoreo remoto y continuo del estado del paciente"]:::causa
    CD5 --> PC


    %% ==========================================
    %% --- EFECTOS (Ramas - Parte Superior) ---
    %% ==========================================

    %% Eje 1: Diseño y Adaptación
    PC --> ED1["EFECTO DIRECTO\nMala adaptación progresiva del paciente a la prótesis"]:::efectoDir
    ED1 --> EI1["EFECTO INDIRECTO\nDificultad en la identificación temprana de complicaciones y molestias"]:::efectoInd
    EI1 --> CAT1["SEGUIMIENTO MÉDICO"]:::cat

    %% Eje 2: Uso y Com

