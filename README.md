# FreeStreamer — ricette

Ricette di scraping (config JSON) usate dall'app **FreeStreamer** per aggiornare i siti
supportati **senza pubblicare una nuova release**.

L'app scarica questi file quando `manifest.json` qui ha una `version` più alta di quella
inclusa nell'APK installato, e li applica al posto delle ricette bundlate (con fallback
a quelle bundlate se un file manca o è malformato).

Contiene **solo** le ricette (già presenti in ogni APK distribuito): il codice
sorgente dell'app è in un repository privato separato.

⚠️ **Regola:** a ogni modifica di una ricetta, incrementa `version` in `manifest.json`.
