# 🏠 HA Blueprints

Raccolta di blueprint pronti all'uso per [Home Assistant](https://www.home-assistant.io/) — automazioni facilmente importabili e personalizzabili tramite la UI, senza scrivere YAML.

![GitHub last commit](https://img.shields.io/github/last-commit/luigi-regolo/ha-blueprints)
![GitHub License](https://img.shields.io/github/license/luigi-regolo/ha-blueprints)

## 📋 Indice

- [Sicurezza](#-sicurezza)
- [Illuminazione](#-illuminazione)
- [Come importare un blueprint](#️-come-importare-un-blueprint)
- [Contribuire](#-contribuire)

---

## 🔒 Sicurezza

### Attiva allarme all'uscita di casa

Quando la persona selezionata esce dalla zona casa, se l'allarme è disinserito, inserisce automaticamente l'allarme, spegne luci e media player (con script opzionale, es. attivazione NVR).

**Richiede:** un'entità `person`, un pannello `alarm_control_panel`

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/luigi-regolo/ha-blueprints/main/automation/sicurezza/attiva-allarme-uscita-casa.yaml)

---

## 💡 Illuminazione

### Accendi luce su apertura porta (di notte)

Accende una luce quando la porta collegata si apre, solo se siamo tra tramonto e alba.

**Richiede:** un sensore porta (`binary_sensor`, device_class door), una luce target

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/luigi-regolo/ha-blueprints/main/automation/illuminazione/luce-apertura-porta.yaml)

### Spegni luce su assenza movimento (porta chiusa, di notte)

Spegne una luce dopo un periodo configurabile di assenza movimento, se la porta collegata è chiusa e siamo tra tramonto e alba.

**Richiede:** un sensore di movimento, un sensore porta, una luce target

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/luigi-regolo/ha-blueprints/main/automation/illuminazione/spegni-luce-assenza-movimento.yaml)

---

## ⬇️ Come importare un blueprint

**Metodo rapido:** clicca il bottone "Import Blueprint" sotto l'automazione che ti interessa.

**Metodo manuale:**
1. Apri Home Assistant
2. Vai su **Impostazioni** → **Automazioni e scene** → tab **Blueprint**
3. Clicca **Importa blueprint**
4. Incolla l'URL raw del file `.yaml` desiderato da questo repository
5. Clicca **Anteprima**, poi **Importa blueprint**
6. Crea una nuova automazione basata sul blueprint e configura i campi richiesti

## 📄 Licenza

Distribuito sotto licenza MIT — vedi [LICENSE](LICENSE) per i dettagli.
