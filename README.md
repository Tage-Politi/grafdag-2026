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
Hent det vi skal snakke om:
```
~> git clone git@github.com:Tage-Politi/grafdag-2026.git
```

For å komme på luften:
```
    ~> cd grafdag/
    grafdag> python3 -v venv
    grafdag> . venv/bin/activate
    (venv) grafdag> pip install -r requirements.txt
    (venv) grafdag> jupyter notebook
```

