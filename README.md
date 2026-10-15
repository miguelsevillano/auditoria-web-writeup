# Caso de Estudio: Auditoría Web y Explotación de Vulnerabilidad Server-Side (Unrestricted File Upload)

**Autor:** Miguel Sevillano 
**Nivel:** Practicante / Junior
**Entorno de Laboratorio:** TryHackMe (Red Interna Aislada)
*   **IP Atacante (Local):** `10.64.173.186`
*   **IP Objetivo (Servidor):** `10.64.133.137`

**Objetivo:** Identificar servicios ocultos, evaluar vulnerabilidades en aplicaciones web (Server-Side) y proponer controles de mitigación.

---

## 1. Fase de Reconocimiento y Enumeración
Se inició la auditoría desde el equipo atacante (`10.64.173.186`) con un escaneo de puertos sobre la dirección IP objetivo utilizando `Nmap` para mapear la superficie de ataque y evadir restricciones de ping (`-Pn`).

**Comando ejecutado:**
```bash
nmap -sV -sC -p 1-5000 -T4 -Pn 10.64.133.137