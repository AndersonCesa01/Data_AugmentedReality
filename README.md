# Dataset README

## Overview

This repository contains two survey datasets collected as part of research projects evaluating visitor experiences with **Augmented Reality (AR)** in cultural and natural heritage contexts in Colombia. Both studies measure how AR technology affects visitor engagement, emotional response, learning, and satisfaction.

---

## File 1: `Encuesta_al_28_06__1-79_.xlsx`

### Context

Survey collected at the **Tropicario** of the **Jardín Botánico de Bogotá (JBB)** — the Bogotá Botanical Garden's tropical ecosystem exhibit. Visitors used QR codes during their tour to interact with AR overlays showcasing Colombian flora and fauna species.

### Population

- **n = 79 respondents** (IDs 1–80, with one gap)
- Nationality: Primarily Colombian, with international visitors from El Salvador, Honduras, Panama, Costa Rica, Mexico, Spain, Dominican Republic, Venezuela, and the USA
- Age groups: 15–29, 30–42, 43–56 years old
- Gender: Male / Female

### Structure

| Column Category | Description |
|---|---|
| `ID` | Respondent identifier |
| `Hora de inicio / finalización` | Survey start and end timestamps (Excel serial format) |
| `Correo electrónico` | Email (anonymized — all entries are `anonymous`) |
| `Consentimiento informado` | Informed consent confirmation |
| `¿Tiene conocimiento sobre el Tropicario?` | Prior knowledge of the Tropicario (Yes/No) |
| `¿Es visitante recurrente del JBB?` | Recurrent visitor of the Botanical Garden (Yes/No) |
| `Uso de QR con realidad aumentada` | Whether the visitor used the AR QR codes during the tour |
| **Pre-experience items (Likert 1–5)** | Environmental awareness, relevance of conservation, familiarity with AR, trust in technology, expected positive emotions |
| **During/post-experience items (Likert 1–5)** | Novelty, authenticity, immersion, engagement, flow, trust, ease of access, ease of use, learning, emotional impact, connection to JBB, motivation, perception change, expectation fulfillment, satisfaction, recommendation |
| `Sugerencias de mejora` | Open-ended improvement suggestions |
| `Género` | Gender |
| `Nacionalidad` | Nationality |
| `Edad` | Age group |

### Likert Scale

All rated items use a **1–5 scale** (1 = strongly disagree / very low, 5 = strongly agree / very high).

### Notes

- Two near-duplicate satisfaction/recommendation columns appear at the end (likely a form versioning artifact)
- Some respondents did not use the AR feature, creating natural comparison groups
- Timestamps are stored as Excel numeric serial dates

---

## File 2: `Base_de_datos_expo_casa_obeso.xlsx`

### Context

Survey collected at the **"Expo Casa Obeso"** art exhibition, centered on **Potrero Grande** — a neighborhood (commune 21) in Cali, Colombia with a predominantly Afro-Colombian population. The exhibition featured murals and illustrations by local artists, enhanced with AR overlays accessible via mobile device. The study examines how AR affects community identity, emotional connection, and cultural appreciation.

### Population

- **n = 146 respondents** (rows 1–146, including some incomplete entries)
- Collected in two phases: the first ~78 rows include qualitative open-ended responses; rows 79–146 contain only quantitative scores
- Respondents include both community members from Potrero Grande and outside visitors
- Age range: 13–79 years old
- Location: Primarily from Cali comunas, with some visitors from Bogotá, Medellín, and international locations

### Structure

| Column | Description |
|---|---|
| `#` (row) | Entry number |
| `Identificación` | Gender code (1 = Male, 2 = Female) |
| `Edad` | Age (in years) |
| `Comuna` | Cali commune of residence (numeric; "No" = outside Cali) |
| `Palabras sobre PG` | Open-ended: Words the visitor associates with Potrero Grande (pre-experience) |
| `Pertenece Potrero` | Community membership (1 = belongs to Potrero Grande, 2 = does not) |
| `Familiarizado con personajes de PG` | Familiarity with notable figures from Potrero Grande (Likert 0–5) |
| `Conectado con la comunidad de PG` | Personal connection to the community (Likert 0–5) |
| `Relevante preservar historia de PG` | Perceived relevance of preserving PG history (Likert 1–5) |
| `Espero profundizar entendimiento (AR)` | Expected learning through AR (Likert 1–5) |
| `Espero experimentar emociones positivas` | Expected positive emotions (Likert 1–5) |
| `AR como forma valiosa de aprender` | AR as a valuable learning tool (Likert 1–5) |
| **Emotional state columns (×4)** | Open-ended: Emotional state before and after interacting with each of two artworks |
| `AR impacto positivo en exposiciones` | AR has a positive impact on art exhibitions (Likert 0–5) |
| `Satisfecho con experiencia AR` | Satisfaction with the AR experience (Likert 0–5) |
| `Motivado a participar en actividades comunitarias` | Motivation to engage with community activities (Likert 0–5) |
| `Conexión emocional con PG aumentó` | Increased emotional connection to PG community (Likert 0–5) |
| `Recomendaría la experiencia AR` | Likelihood to recommend (Likert 0–5) |
| `Palabras después de la experiencia` | Open-ended: Words associated with Potrero Grande after the experience |

### Notes

- Rows 1–78 contain rich qualitative data (emotional reactions, open-ended descriptions) in addition to Likert scores
- Rows 79–146 contain only quantitative Likert responses (likely a second phase of data collection with a shorter instrument)
- Missing values and `0` entries are common; treat `0` as missing/non-response rather than a valid score where context suggests it
- Community membership (column `Pertenece Potrero`) enables insider vs. outsider visitor comparisons

---

## Thematic Overlap Between Files

Both datasets share a common theoretical framework around **AR-enhanced cultural experiences**, measuring:

- **Expectation vs. fulfillment** — pre/post comparisons
- **Emotional engagement** — immersion, flow, positive affect
- **Knowledge acquisition** — self-reported learning
- **Behavioral intention** — recommendation, future participation
- **Overall satisfaction**

---

## Suggested Use

- Likert items can be aggregated into latent constructs (e.g., immersion, satisfaction, learning) using factor analysis or reliability testing (Cronbach's alpha)
- Qualitative columns in File 2 are suitable for thematic or sentiment analysis
- Demographic and context variables (nationality, age, community membership, AR usage) can serve as grouping variables for comparative analysis
- The two datasets can be analyzed separately or used for cross-context comparison of AR effectiveness

---

## Language

All survey items, responses, and open-ended text are in **Spanish**.
