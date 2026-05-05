# DESCO API Swagger Docs

![DESCO Logo](assets/desco-logo.png)

Interactive Swagger documentation for the Dhaka Electric Supply Company (DESCO) REST API. Browse and explore API endpoints for customer management, billing, meter readings, connection applications, and outage reporting — all in one place.

> **Disclaimer:** This is an **unofficial, community-maintained project**. All API definitions have been collected from openly available APIs and publicly accessible information on the internet. This project is not affiliated with, endorsed by, or associated with DESCO in any way.

---

## Preview

Open `index.html` in a browser via a local HTTP server to view the interactive Swagger UI.

## Getting Started

No installation or build step required. This is a pure static project.

**Serve locally with Python:**

```bash
python3 -m http.server 8080
```

Then open [http://localhost:8080](http://localhost:8080) in your browser.

**Or with Node.js:**

```bash
npx serve .
```

## Project Structure

```
desco-api-swagger-docs/
├── index.html        # Entry point — loads Swagger UI
├── swagger.json      # OpenAPI 3.0 API specification
├── style.css         # Custom DESCO branding
└── assets/
    └── desco-logo.png
```

## API Coverage

| Tag         | Endpoints                                              |
|-------------|--------------------------------------------------------|
| Auth        | Register, Login, Logout, Refresh Token                 |
| Customers   | List, Get, Update, Delete                              |
| Bills       | List, Get, Pay                                         |
| Meters      | List, Get, Readings (list & submit)                    |
| Connections | List, Apply, Get, Update Status                        |
| Outages     | List, Report, Get                                      |

Authentication uses **JWT Bearer tokens**. Secured endpoints require an `Authorization: Bearer <token>` header.

## Tech Stack

- [Swagger UI v5](https://swagger.io/tools/swagger-ui/) — interactive API browser
- [OpenAPI 3.0](https://spec.openapis.org/oas/v3.0.3) — API specification format
- Plain HTML, CSS, JavaScript — no framework, no build tools

## Author

**Abid Hasan**
- GitHub: [@abidtkg](https://github.com/abidtkg)

## License

This project is open source and available under the [MIT License](LICENSE).
