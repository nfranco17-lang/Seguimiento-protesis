```mermaid
graph BT

    %% PROBLEMA CENTRAL
    PC["<b>PROBLEMA CENTRAL</b><br/>Inadecuado seguimiento y registro de la evolución<br/>de pacientes con prótesis"]

    %% CAUSAS INDIRECTAS
    CI1["<b>CAUSA INDIRECTA</b><br/>Ausencia de herramientas digitales simples<br/>para el autoreporte diario"]
    CI2["<b>CAUSA INDIRECTA</b><br/>Historial de seguimiento manual,<br/>disperso o en papel"]
    CI3["<b>CAUSA INDIRECTA</b><br/>Bajo uso de sistemas o sensores<br/>(IoT/wearables) entre consultas"]

    %% CAUSAS DIRECTAS
    CD1["<b>CAUSA DIRECTA</b><br/>Registro ineficaz de dolor,<br/>comodidad y frecuencia de uso"]
    CD2["<b>CAUSA DIRECTA</b><br/>Dependencia exclusiva de citas<br/>presenciales muy espaciadas"]
    CD3["<b>CAUSA DIRECTA</b><br/>Ausencia de tecnología de monitoreo<br/>remoto del estado del paciente"]

    %% EFECTOS DIRECTOS
    ED1["<b>EFECTO DIRECTO</b><br/>Mala adaptación progresiva y<br/>malestar físico continuo"]
    ED2["<b>EFECTO DIRECTO</b><br/>Dificultad en la identificación<br/>temprana de molestias y fallas"]
    ED3["<b>EFECTO DIRECTO</b><br/>Casos de desajuste protésico<br/>sin intervención oportuna"]

    %% EFECTOS INDIRECTOS
    EI1["<b>EFECTO INDIRECTO</b><br/>Abandono o uso intermitente de la<br/>prótesis por parte del paciente"]
    EI2["<b>EFECTO INDIRECTO</b><br/>Aparición de complicaciones graves<br/>(úlceras por presión, lesiones)"]
    EI3["<b>EFECTO INDIRECTO</b><br/>Sobrecostos en el sistema por<br/>reingresos o intervenciones de urgencia"]

    %% CATEGORÍAS TEMÁTICAS (ENCABEZADOS)
    CAT1["<b>ADAPTACIÓN Y CONFORT</b>"]
    CAT2["<b>SALUD Y PREVENCIÓN</b>"]
    CAT3["<b>GESTIÓN CLÍNICA</b>"]

    %% CONEXIONES DE CAUSAS (Abajo -> Centro)
    CI1 --> CD1 --> PC
    CI2 --> CD2 --> PC
    CI3 --> CD3 --> PC

    %% CONEXIONES DE EFECTOS (Centro -> Arriba)
    PC --> ED1 --> EI1 --> CAT1
    PC --> ED2 --> EI2 --> CAT2
    PC --> ED3 --> EI3 --> CAT3

    %% ESTILOS VISUALES
    style PC fill:#2d3748,stroke:#1a202c,stroke-width:2px,color:#fff
    
    style CD1 fill:#81e6d9,stroke:#319795,color:#1a202c
    style CD2 fill:#81e6d9,stroke:#319795,color:#1a202c
    style CD3 fill:#81e6d9,stroke:#319795,color:#1a202c

    style CI1 fill:#e2e8f0,stroke:#cbd5e0,color:#2d3748
    style CI2 fill:#e2e8f0,stroke:#cbd5e0,color:#2d3748
    style CI3 fill:#e2e8f0,stroke:#cbd5e0,color:#2d3748

    style ED1 fill:#9ae6b4,stroke:#38a169,color:#1a202c
    style ED2 fill:#9ae6b4,stroke:#38a169,color:#1a202c
    style ED3 fill:#9ae6b4,stroke:#38a169,color:#1a202c

    style EI1 fill:#e2e8f0,stroke:#cbd5e0,color:#2d3748
    style EI2 fill:#e2e8f0,stroke:#cbd5e0,color:#2d3748
    style EI3 fill:#e2e8f0,stroke:#cbd5e0,color:#2d3748

    style CAT1 fill:#2f855a,stroke:#22543d,color:#fff
    style CAT2 fill:#2f855a,stroke:#22543d,color:#fff
    style CAT3 fill:#2f855a,stroke:#22543d,color:#fff

