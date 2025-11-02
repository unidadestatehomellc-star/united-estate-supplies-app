
# United Estate Supplies — Starter App (Flask)

App web funcional para catálogo de productos (computadoras/suministros) y órdenes simples.
Listo para ejecutar en local con Python 3.10+.

## Características
- Catálogo de productos (crear/editar/eliminar desde panel admin)
- Búsqueda por nombre/sku
- Carrito sencillo y creación de orden
- Listado de órdenes (admin)
- SQLite (archivo `app.db`) — sin dependencias externas
- UI básica con Bootstrap (CDN)

## Requisitos
- Python 3.10+
- pip

## Instalación (Mac/Windows/Linux)
```bash
cd united_estate_supplies_app
python -m venv .venv
source .venv/bin/activate  # En Windows: .venv\Scripts\activate
pip install -r requirements.txt
python app.py
```
Visita: http://127.0.0.1:5000

### Acceso admin
- Ir a: http://127.0.0.1:5000/admin
- PIN por defecto: 2468 (puedes cambiarlo en `.env`)

## Estructura
```
united_estate_supplies_app/
  app.py
  db.py
  models.py
  forms.py
  requirements.txt
  .env
  templates/
  static/
```

## Despliegue sugerido
- Render.com, Railway, u otra opción gratuita. Ajusta `PORT`/`HOST` según el proveedor.

## Próximos pasos
- Agregar autenticación real (usuarios/roles)
- Exportar/descargar órdenes en CSV
- Integrar pasarela de pago (PayPal/Stripe) si se desea
- API REST para integraciones (Shopify, DOBA, etc.)
```
