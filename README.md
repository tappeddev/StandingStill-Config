# StandingStill-Config

Durch die `config.json` kann man nun die Konfiguration in der StandingStill-App anpassen. Dazu wird der Github Raw-Content geladen (https://raw.githubusercontent.com/tappeddev/StandingStill-Config/refs/heads/main/config.json). Voraussetzung dafür ist, dass der Nutzer bei App-Start eine Verbindung zum Internet besitzt. Durch Drücken auf den Start-Button wird die Konfiguration auch nochmal geladen. Falls diese beiden Requests nicht erfolgreich waren, wird die Default Einstellung verwendet:
```json
{
   "samplingRateStandingStillDataMillis": 3000,
   "thresholdStd": 0.09,
   "thresholdStd": 0.4,
   "samplingRateSensorDataMillis": 200
}
```

⚠️ Es kann sein, dass die aktualisierte Konfiguration erst nach ca. 5 Minuten zur Verfügung steht, weil bei Github ein Caching verwendet wird, welches das direkte Aktualisieren des Raw-Contents verzögert.

# Valide Werte für die Konfiguration

1. `samplingRateStandingStillDataMillis`

Min: 0

Max: ∞

2. `samplingRateSensorDataMillis`

[0, 20, 66, 200]

