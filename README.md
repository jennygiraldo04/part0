# part0

### Ejemplo de un diagrama básico

```markdown
```mermaid
graph TD;
    A[Usuario] --> B[Login];
    B --> C{Acceso correcto?};
    C -->|Sí| D[Dashboard];
    C -->|No| E[Mensaje de error];
