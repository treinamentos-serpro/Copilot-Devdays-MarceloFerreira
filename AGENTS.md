# AGENTS.md

## Mandatory checklist before completion
- Run lint if configured.
- Run the build: `cd socops && ./mvnw clean package`
- Run the tests: `cd socops && ./mvnw test`
- Confirm the app still starts: `cd socops && ./mvnw spring-boot:run`

## Scope
This repo contains a Spring Boot social bingo app with Thymeleaf views, utility-based CSS, and business logic in `socops/src/main/java/com/socops`.

## Rules
- Keep changes small and focused.
- Put business logic in service/model classes, not controllers.
- Prefer readable Java and explicit names.
- Use the existing utility CSS patterns in `socops/src/main/resources/static/css/app.css`.
- Avoid generic AI styling; keep the UI distinctive and intentional.
- Prefer test-driven fixes when behavior changes.

## Workflow
1. Inspect the issue and root cause.
2. Add or update a failing test when practical.
3. Implement the minimal fix.
4. Re-run validation.
5. Summarize the change and evidence.

## Project layout
- `socops/` — app
- `socops/src/main/java/com/socops/` — Java app code
- `socops/src/main/resources/templates/` — Thymeleaf pages
- `socops/src/main/resources/static/css/` — CSS utilities
- `socops/src/test/java/` — tests
- `workshop/` — lab materials

## Notes
- The app is a Spring Boot service with endpoints served from the controller layer.
- Keep implementation aligned with the workshop and existing project structure.
