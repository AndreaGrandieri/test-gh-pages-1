# clock

## tl;dr

Il seguente modulo mostra la data e l'ora correnti.

---

## config.js fragment

```js
{
    module: "clock",
    position: "top_left",
    config: {
        timeFormat: 24,
        displaySeconds: true,
        showDate: true,
        displayType: 'digital',
        timezone: 'Europe/Rome',
    }
}
```

---

## Propriet√† (config section)

| Propriet√†        | Tipo      | Valori                                                                                       | Valore Default        | Inderogabilit√† | Descrizione                                                         |
| ---------------- | --------- | -------------------------------------------------------------------------------------------- | --------------------- | -------------- | ------------------------------------------------------------------- |
| `timeFormat`     | `Number`  | `12` <br> `24`                                                                               | _`config.timeFormat`_ | `OPTIONAL`     | Formato dell'ora (12 o 24 ore)                                      |
| `displaySeconds` | `Boolean` | `true`: visualizzazione secondi attivato. <br> `false`: visualizzazione secondi disattivato. | `true`                | `OPTIONAL`     | Attiva / disattiva visualizzazione secondi.                         |
| `showDate`       | `Boolean` | `true`: visualizzazione data attivato. <br> `false`: visualizzazione data disattivato.       | `true`                | `OPTIONAL`     | Attiva / disattiva visualizzazione data.                            |
| `displayType`    | `String`  | `digital` <br> `analog` <br> `both`                                                          | `"digital"`           | `OPTIONAL`     | Visualizzazione orario come orologio analogico, digitale o entrambi |
| `timezone`       | `String`  | Qui puoi trovare / cercare tutte le possibili zone: https://momentjs.com/timezone/.          | `---`                 | `REQUIRED`     | Zona di cui mostrare l'ora                                          |

---

## Notifiche

Le notifiche sono uno strumento utilizzato dai moduli per comunicare con:

- L'OS del MagicMirror
- Altri moduli
- Attori umani

| Notifica       | Direzione | Trigger               | Payload _(inline js)_ | Descrizione |
| -------------- | --------- | --------------------- | --------------------- | ----------- |
| `CLOCK_SECOND` | `OUT`     | Ogni secondo passato. | `second_value`        | ---         |
| `CLOCK_MINUTE` | `OUT`     | Ogni munuto passato.  | `minute_value`        | ---         |

---

## Screenshots

Questa √® la visualizzazione del modulo in situazione di funzionamento corretto:

![clock.png](../../../assets/clock/clock.png)

---
