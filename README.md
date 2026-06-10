# fastAPI
![FastAPI Logo](https://fastapi.tiangolo.com/img/logo-margin/logo-teal.png)

## Descrizione

Progetto di esempio in Python che illustra l'utilizzo della libreria **FastAPI** per la creazione di API RESTful.

Il server espone un endpoint `GET /` che restituisce un semplice messaggio JSON di benvenuto:

```json
{
  "real": "python",
  "saluto": "hello world"
}
```

## Struttura del progetto

```
fastAPI/
├── fastAPI/
│   ├── __init__.py
│   └── main.py        # Definizione dell'app FastAPI e degli endpoint
├── all-requirements.txt
└── README.md
```

## Requisiti

- Python 3.10+
- Dipendenze elencate in `all-requirements.txt` (FastAPI, Uvicorn, Pydantic, ecc.)

## Installazione

1. Clona il repository:
   ```bash
   git clone <url-repository>
   cd fastAPI
   ```

2. Crea e attiva un ambiente virtuale:
   ```bash
   python -m venv .venv
   .venv\Scripts\activate      # Windows
   # source .venv/bin/activate # Linux/macOS
   ```

3. Installa le dipendenze:
   ```bash
   pip install -r all-requirements.txt
   ```

## Avvio del server

```bash
uvicorn fastAPI.main:app --reload
```

Il server sarà disponibile su: [http://127.0.0.1:8000](http://127.0.0.1:8000)

## Endpoint disponibili

| Metodo | Path | Descrizione           | Risposta                                          |
|--------|------|-----------------------|---------------------------------------------------|
| GET    | `/`  | Endpoint di benvenuto | `{"real": "python", "saluto": "hello world"}`     |

## Documentazione interattiva

FastAPI genera automaticamente la documentazione delle API:

- **Swagger UI**: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)
- **ReDoc**: [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc)

## Avvio da VS Code

Il progetto include una configurazione di debug in `.vscode/launch.json`.  
Usa il profilo **"uvicorn"** per avviare il server direttamente dall'editor con il tasto `F5`.

## Licenza

Questo progetto è distribuito sotto licenza **MIT**. Consulta il file [LICENSE](LICENSE) per i dettagli.

