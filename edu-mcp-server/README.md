# EDU MCP Server

Servidor MCP (Model Context Protocol) que expone funcionalidades core del módulo EDU para consumo por agentes externos.

## Setup

```bash
pip install -r edu-mcp-server/requirements.txt
```

## Configuración en VS Code

Agregar a `.vscode/mcp.json`:

```json
{
  "servers": {
    "edu": {
      "type": "stdio",
      "command": "python",
      "args": ["salida/edu-standalone/edu-mcp-server/server.py"]
    }
  }
}
```

## Tools expuestos

| Tool | Descripción |
|------|-------------|
| `edu.search_memory` | Buscar en la memoria colectiva (SQLite FTS5) |
| `edu.validate_plan` | Validar un plan de filminas JSON |
| `edu.get_slide_template` | Obtener template de slide por tipo |
| `edu.search_knowledge` | Buscar en ChromaDB knowledge base |
| `edu.anonimizar_documento` | Anonimizar PII con Microsoft Presidio → `anon_mapping.json` local |
| `edu.generar_oficio_docx` | Generar oficio judicial `.docx` desde salida estructurada de ChatGPT |
| `edu.generar_sentencia_docx` | Generar sentencia `.docx` en lenguaje claro, con des-anonimización opcional |

## Dependencias adicionales (tools de documentos judiciales)

```bash
pip install python-docx presidio-analyzer presidio-anonymizer
python -m spacy download es_core_news_lg
```

## Uso

El servidor se inicia automáticamente cuando VS Code lo necesita (configuración stdio).

Para prueba manual:
```bash
python edu-mcp-server/server.py
```
