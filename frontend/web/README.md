# TELORA web interface

The customer view and the admin console are served by `backend.api.app` and call its
same-origin FastAPI routes through `js/api.js`.

From the repository root:

```bash
python -m pip install -r requirements.txt
uvicorn backend.api.app:app --reload
```

Open `http://127.0.0.1:8000`.

- **Customer:** pick a demo customer, build a solution (needs → levels → budget), follow
  live progress, compare the solutions, then apply or cancel.
- **Admin:** Overview, Requests (full journey of each request), Customers, Agents, and Catalog.

Customer selection is a prototype Demo Mode session. It does not authenticate the person
using the browser, and the admin console has no login in this prototype.
