# grafdag-2026

## Nødvendige forberedelser

### Intune PC
Søke i `http://tilgang` om **Local Admin**.

Når det er gjort, start programmet `MakeMeAdmin`, og  gå til Firmaportalen og last ned "Ubuntu 24.04 LTS".

Deretter
```
sudo apt install podman
```

### Intune Mac
```
brew install podman
podman machine init
podman machine start
```
Fordi du ikke skal åpne porter under 1024 kan du ignorere advarselen:
```
This machine is currently configured in rootless mode.
```

## Programvaren


For å komme på luften:
```
    ~> python3 -v venv
    ~> . venv/bin/activate
    (venv) ~> pip install -r requirements.txt
```
