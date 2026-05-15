---
name: workspace
description: Workspace-specific guidance for the my-soc-ops-java Spring Boot repository.
---

# Workspace Instructions

## Mandatory development checklist

- [ ] Lint / style checks
- [ ] Build: `cd socops && ./mvnw clean package`
- [ ] Test: `cd socops && ./mvnw test`

## Quick start

- App root: `socops/`
- Runtime: Java 21
- Use the Maven wrapper: `./mvnw`
- Run locally: `cd socops && ./mvnw spring-boot:run`
- Open `http://127.0.0.1:8080/`

## Key files

- `socops/src/main/java/com/socops/SocOpsApplication.java`
- `socops/src/main/java/com/socops/web/BingoRestController.java`
- `socops/src/main/java/com/socops/service/BoardAssembler.java`
- `socops/src/main/resources/templates/game.html`
- `socops/src/main/resources/static/css/app.css`
- `socops/src/test/java/com/socops/service/BoardAssemblerTests.java`

## Repo conventions

- Keep backend logic in `service/` and `model/`
- Keep endpoints in `web/`
- Keep markup in `templates/` and styles in `static/css/`
- Add tests under `socops/src/test/java/`
- `.github/prompts/` holds prompt files and `.github/instructions/` holds repo guidance
