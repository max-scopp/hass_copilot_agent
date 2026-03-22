# Home Assistant Labels & Categories Reference

## Naming Conventions
- **Entity IDs**: English (e.g., `light.kitchen_ceiling_main`)
- **Display text** (labels, categories, friendly names): German
- **Categories**: Use emoji prefix + German name
- **Labels**: German name, no emoji in label name (emoji goes in icon field)

---

## Labels (Create in HA: Settings → Labels)

| Label Name        | Icon                    | Color  | Notes                        |
| ----------------- | ----------------------- | ------ | ---------------------------- |
| Beleuchtung       | `mdi:lightbulb`         | Yellow | Lighting automations         |
| Bewegung          | `mdi:motion-sensor`     | Blue   | Motion-activated             |
| Jalousien         | `mdi:window-shade`      | Purple | Covers/shutters              |
| Sonnenaufgang     | `mdi:sunrise`           | Orange | Sunrise-based                |
| Sonnenuntergang   | `mdi:sunset`            | Orange | Sunset-based                 |
| Türen             | `mdi:door`              | Gray   | Door sensors/automations     |
| Eingang           | `mdi:door-front`        | Brown  | Entry-specific               |
| Steuerung         | `mdi:remote`            | Teal   | Manual/remote controls       |
| Alarme            | `mdi:alarm`             | Yellow | Alarm/wake-up automations    |
| Anwesenheit       | `mdi:home-account`      | Green  | Presence-based               |
| Sicherheit        | `mdi:shield-account`    | Red    | Security automations         |
| Abends            | `mdi:moon`              | Indigo | Time-based (nighttime)       |
| Belüftung         | `mdi:fan`               | Cyan   | Ventilation/humidity         |
| Müll              | `mdi:trash-can`         | Brown  | Garbage collection reminders |
| Tägliche Routine  | `mdi:calendar-check`    | Blue   | Daily recurring automations  |
| Garten/Energie    | `mdi:lightning-bolt`    | Yellow | Garden/energy management     |
| Kostenoptimierung | `mdi:cash-multiple`     | Green  | Cost/energy optimization     |
| Medien            | `mdi:television`        | Purple | Media player automations     |
| Reinigung         | `mdi:robot-vacuum`      | Green  | Cleaning automations         |
| 3D-Druck          | `mdi:printer-3d`        | Gray   | 3D printer notifications     |
| VR/Gaming         | `mdi:vr-box`            | Purple | VR/gaming setup              |
| Klimakontrolle    | `mdi:thermometer-check` | Orange | Temperature/climate control  |

---

## Categories (One per automation)

Categories are emoji-prefixed display names used to organize automations in HA UI:

| Category         | Icon                    | Color  | Used For                        |
| ---------------- | ----------------------- | ------ | ------------------------------- |
| 💡 Beleuchtung    | `mdi:lightbulb`         | Yellow | Lighting automations            |
| 🎚️ Jalousien      | `mdi:window-shade`      | Purple | Cover/shutter automations       |
| 🛡️ Sicherheit     | `mdi:shield-account`    | Red    | Security automations            |
| 🏠 Anwesenheit    | `mdi:home-account`      | Green  | Presence-based automations      |
| 🤖 Reinigung      | `mdi:robot-vacuum`      | Green  | Cleaning automations            |
| ⚡ Garten/Energie | `mdi:lightning-bolt`    | Yellow | Garden/energy automations       |
| ⏰ Alarme         | `mdi:alarm`             | Yellow | Alarm/wake-up automations       |
| ☀️ Klimakontrolle | `mdi:thermometer-check` | Orange | Climate/temperature automations |
| 💨 Belüftung      | `mdi:fan`               | Cyan   | Ventilation automations         |
| 🗑️ Müll           | `mdi:trash-can`         | Brown  | Garbage collection automations  |
| 🎛️ Steuerung      | `mdi:remote`            | Teal   | Manual control automations      |
| 🖨️ 3D-Druck       | `mdi:printer-3d`        | Gray   | 3D printer automations          |
| 💻 VR/Gaming      | `mdi:vr-box`            | Purple | VR/gaming automations           |

---

## Key Principles

1. **Illuminance checks = Add "Abends" label** — Any automation with a brightness/illuminance condition checking for darkness should get the 🌙 Abends label for consistency
2. **Multi-label automations** — One automation can have 2-3 labels to group related items across HA
3. **One category per automation** — Categories organize within their type; labels organize across types
4. **German naming** — All user-facing text in German for consistency
5. **Icons not emojis in labels** — Use `mdi:` icon format, emoji goes in display text as prefix

---

## To Apply in HA UI

1. Create all 22 labels with icons/colors
2. Assign 1 category per automation
3. Assign labels (multi-select) per automation
4. Use for filtering and organization across HA dashboard
