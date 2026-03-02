# grafdag-2026

## Nødvendige forberedelser

### Intune PC
Søke i `http://tilgang` om **Local Admin**.

Når det er innvilget, start programmet `MakeMeAdmin`, og  gå til
Firmaportalen og last ned "Ubuntu 24.04 LTS"; tar litt tid.

Etter den obligatoriske `sudo apt update` og `sudo apt upgrade` kjører du 
```
sudo apt install podman
```
Fordi du ikke skal åpne porter under 1024 kan du ignorere denne advarselen:
```
This machine is currently configured in rootless mode.
```

### Intune Mac
Rykter forteller at dette er det som er nødvendig:
```
brew install podman
podman machine init
podman machine start
```
Fordi du ikke skal åpne porter under 1024 kan du ignorere denne advarselen:
```
This machine is currently configured in rootless mode.
```

## Programvaren

I en terminal, som på Intune er en `Ubuntu` skal du først
ente det vi skal snakke om:
```
~> git clone https://github.com/Tage-Politi/grafdag-2026.git
```

For å komme på luften:
1. Først lage en Python-omgivelse;
2. Aktivere den;
3. Fylle den med programvare, og
4. Starte og opprette forbindelse tli *notebook*.

```
    ~> cd grafdag-2026
    grafdag> python3 -v venv venv
    grafdag> . venv/bin/activate
    (venv) grafdag> pip install -r requirements.txt
    (venv) grafdag> jupyter notebook
```
Blant all teksten finner du:
```
    Or copy and paste one of these URLs:
        http://localhost:8888/tree?token=75a6c8b174f0729a9b81071285e4fbaa11c1c5c737162c46
        http://127.0.0.1:8888/tree?token=75a6c8b174f0729a9b81071285e4fbaa11c1c5c737162c46
```
Lim URL'en inn i din fa voritt-nettleser.