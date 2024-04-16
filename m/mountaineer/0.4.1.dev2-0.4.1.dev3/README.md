# Comparing `tmp/mountaineer-0.4.1.dev2.tar.gz` & `tmp/mountaineer-0.4.1.dev3.tar.gz`

## Comparing `mountaineer-0.4.1.dev2.tar` & `mountaineer-0.4.1.dev3.tar`

### file list

```diff
@@ -1,259 +1,259 @@
--rw-r--r--   0     1001      127      269 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src_go/Cargo.toml
--rw-r--r--   0     1001      127     1995 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src_go/build.rs
--rw-r--r--   0     1001      127     5657 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src_go/go/js_build.go
--rw-r--r--   0     1001      127      168 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src_go/go.mod
--rw-r--r--   0     1001      127      376 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src_go/go.sum
--rw-r--r--   0     1001      127     5750 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src_go/src/lib.rs
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.4.1.dev2/Cargo.toml
--rw-r--r--   0     1001      127      133 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/.git-blame-ignore-revs
--rw-r--r--   0     1001      127      138 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/.gitattributes
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/.github/README_SCRIPTS.md
--rw-r--r--   0     1001      127    14036 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/.github/poetry.lock
--rw-r--r--   0     1001      127      767 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/.github/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/.github/scripts/__init__.py
--rw-r--r--   0     1001      127     3032 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/.github/scripts/__tests__/test_update_version.py
--rw-r--r--   0     1001      127     2181 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/.github/scripts/check_dependencies.py
--rw-r--r--   0     1001      127     3382 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/.github/scripts/update_version.py
--rw-r--r--   0     1001      127     1321 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/.github/workflows/publish_docs.yml
--rw-r--r--   0     1001      127    19767 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/.github/workflows/test.yml
--rw-r--r--   0     1001      127      504 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/.github/workflows/validate.yml
--rw-r--r--   0     1001      127     3404 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/.gitignore
--rw-r--r--   0     1001      127     1750 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/Dockerfile
--rw-r--r--   0     1001      127     1079 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/LICENSE
--rw-r--r--   0     1001      127     4976 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/Makefile
--rw-r--r--   0     1001      127    14891 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/README.md
--rw-r--r--   0     1001      127      105 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/benchmarking/README.md
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/benchmarking/benchmarking/__init__.py
--rw-r--r--   0     1001      127      425 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/benchmarking/benchmarking/simple_render.py
--rw-r--r--   0     1001      127   127093 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/benchmarking/poetry.lock
--rw-r--r--   0     1001      127      291 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/benchmarking/pyproject.toml
--rw-r--r--   0     1001      127      850 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/README.md
--rw-r--r--   0     1001      127        1 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/__init__.py
--rw-r--r--   0     1001      127      775 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/app.py
--rw-r--r--   0     1001      127      489 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/cli.py
--rw-r--r--   0     1001      127      111 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/config.py
--rw-r--r--   0     1001      127        1 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/controllers/__init__.py
--rw-r--r--   0     1001      127     1433 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/controllers/complex.py
--rw-r--r--   0     1001      127      581 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/controllers/detail.py
--rw-r--r--   0     1001      127     1658 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/controllers/home.py
--rw-r--r--   0     1001      127      559 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/controllers/stream.py
--rw-r--r--   0     1001      127       77 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/main.py
--rw-r--r--   0     1001      127      208 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/views/__init__.py
--rw-r--r--   0     1001      127     2261 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/views/app/complex/page.tsx
--rw-r--r--   0     1001      127      453 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/views/app/detail/page.tsx
--rw-r--r--   0     1001      127     2822 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/views/app/home/page.tsx
--rw-r--r--   0     1001      127       59 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/views/app/main.css
--rw-r--r--   0     1001      127      708 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/views/app/stream/page.tsx
--rw-r--r--   0     1001      127   125408 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/views/package-lock.json
--rw-r--r--   0     1001      127      453 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/views/package.json
--rw-r--r--   0     1001      127       83 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/views/postcss.config.js
--rw-r--r--   0     1001      127      161 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/views/tailwind.config.js
--rw-r--r--   0     1001      127   107805 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/poetry.lock
--rw-r--r--   0     1001      127      724 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/ci_webapp/pyproject.toml
--rw-r--r--   0     1001      127     1593 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/README.md
--rw-r--r--   0     1001      127        1 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
--rw-r--r--   0     1001      127     1055 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
--rw-r--r--   0     1001      127     7904 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
--rw-r--r--   0     1001      127      292 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
--rw-r--r--   0     1001      127      816 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
--rw-r--r--   0     1001      127     4277 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/builder.py
--rw-r--r--   0     1001      127     4656 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/cli.py
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
--rw-r--r--   0     1001      127     1383 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/environments/base.py
--rw-r--r--   0     1001      127     4591 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
--rw-r--r--   0     1001      127     1832 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/environments/venv.py
--rw-r--r--   0     1001      127     1336 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/external.py
--rw-r--r--   0     1001      127     1925 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/generation.py
--rw-r--r--   0     1001      127      327 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/io.py
--rw-r--r--   0     1001      127       30 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
--rw-r--r--   0     1001      127      212 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
--rw-r--r--   0     1001      127      190 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
--rw-r--r--   0     1001      127      137 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
--rw-r--r--   0     1001      127      109 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
--rw-r--r--   0     1001      127      170 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/.env
--rw-r--r--   0     1001      127     3373 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
--rw-r--r--   0     1001      127      645 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
--rw-r--r--   0     1001      127       17 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
--rw-r--r--   0     1001      127      767 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
--rw-r--r--   0     1001      127      947 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
--rw-r--r--   0     1001      127      282 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
--rw-r--r--   0     1001      127      227 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
--rw-r--r--   0     1001      127     1702 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
--rw-r--r--   0     1001      127     1124 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
--rw-r--r--   0     1001      127       84 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
--rw-r--r--   0     1001      127      157 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
--rw-r--r--   0     1001      127      208 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
--rw-r--r--   0     1001      127     1219 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
--rw-r--r--   0     1001      127      995 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
--rw-r--r--   0     1001      127       95 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
--rw-r--r--   0     1001      127      524 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
--rw-r--r--   0     1001      127      117 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
--rw-r--r--   0     1001      127      195 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
--rw-r--r--   0     1001      127      332 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
--rw-r--r--   0     1001      127     1493 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
--rw-r--r--   0     1001      127    61104 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/poetry.lock
--rw-r--r--   0     1001      127     1214 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/create_mountaineer_app/pyproject.toml
--rw-r--r--   0     1001      127       30 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/.zed/settings.json
--rw-r--r--   0     1001      127      107 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/README.md
--rw-r--r--   0     1001      127       15 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/CNAME
--rw-r--r--   0     1001      127      310 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/actions.md
--rw-r--r--   0     1001      127      454 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/api_exception.md
--rw-r--r--   0     1001      127       99 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/app-controller.md
--rw-r--r--   0     1001      127      281 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/build_plugins/base.md
--rw-r--r--   0     1001      127       57 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/build_plugins/javascript.md
--rw-r--r--   0     1001      127       62 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/build_plugins/postcss.md
--rw-r--r--   0     1001      127      411 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/cli.md
--rw-r--r--   0     1001      127      376 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/config.md
--rw-r--r--   0     1001      127       61 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/controller.md
--rw-r--r--   0     1001      127       67 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/core_dependencies.md
--rw-r--r--   0     1001      127       66 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/database/config.md
--rw-r--r--   0     1001      127       71 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/database/dependencies.md
--rw-r--r--   0     1001      127       80 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/logging.md
--rw-r--r--   0     1001      127      479 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/render.md
--rw-r--r--   0     1001      127      365 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/ssr.md
--rw-r--r--   0     1001      127      299 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/api/watch_server.md
--rw-r--r--   0     1001      127     9375 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/client_actions.md
--rw-r--r--   0     1001      127      753 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/cma.md
--rw-r--r--   0     1001      127     3021 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/database.md
--rw-r--r--   0     1001      127     4677 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/deploy.md
--rw-r--r--   0     1001      127     7698 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/error_handling.md
--rw-r--r--   0     1001      127     1081 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/index.md
--rw-r--r--   0     1001      127     1541 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/internal/core_library.md
--rw-r--r--   0     1001      127     2156 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/links.md
--rw-r--r--   0     1001      127   365251 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/media/final_todo_list.png
--rw-r--r--   0     1001      127   148261 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/media/ide_typehints.png
--rw-r--r--   0     1001      127   545494 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/media/network_debug.png
--rw-r--r--   0     1001      127   346903 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/media/server_side_rendering.png
--rw-r--r--   0     1001      127     2263 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/metadata.md
--rw-r--r--   0     1001      127     2347 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/postcss.md
--rw-r--r--   0     1001      127    12265 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/quickstart.md
--rw-r--r--   0     1001      127     4875 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/static_analysis.md
--rw-r--r--   0     1001      127     2490 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/structure.md
--rw-r--r--   0     1001      127     1219 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/stylesheets/extra.css
--rw-r--r--   0     1001      127     4080 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/docs/views.md
--rw-r--r--   0     1001      127     1823 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/mkdocs.yml
--rw-r--r--   0     1001      127      109 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/overrides/partials/footer.html
--rw-r--r--   0     1001      127   156250 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/poetry.lock
--rw-r--r--   0     1001      127      479 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/docs_website/pyproject.toml
--rw-r--r--   0     1001      127   675789 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/media/header.png
--rw-r--r--   0     1001      127      954 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/actions/__init__.py
--rw-r--r--   0     1001      127     7884 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/actions/test_fields.py
--rw-r--r--   0     1001      127     9707 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/actions/test_passthrough.py
--rw-r--r--   0     1001      127     9074 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/actions/test_sideeffect.py
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/client_builder/__init__.py
--rw-r--r--   0     1001      127    12565 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/client_builder/test_build_actions.py
--rw-r--r--   0     1001      127     3474 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/client_builder/test_build_links.py
--rw-r--r--   0     1001      127    10097 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/client_builder/test_build_schemas.py
--rw-r--r--   0     1001      127     5001 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/client_builder/test_builder.py
--rw-r--r--   0     1001      127     4153 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/client_builder/test_typescript.py
--rw-r--r--   0     1001      127      319 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/common.py
--rw-r--r--   0     1001      127      497 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/conftest.py
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/database/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/database/dependencies/__init__.py
--rw-r--r--   0     1001      127      208 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/database/dependencies/conftest.py
--rw-r--r--   0     1001      127      801 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/database/dependencies/test_core.py
--rw-r--r--   0     1001      127      627 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/database/test_config.py
--rw-r--r--   0     1001      127      616 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/database/test_sqlmodel.py
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/dependencies/__init__.py
--rw-r--r--   0     1001      127     2567 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/dependencies/test_base.py
--rw-r--r--   0     1001      127      211 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/fixtures/__init__.py
--rw-r--r--   0     1001      127   571338 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
--rw-r--r--   0     1001      127  1638568 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
--rw-r--r--   0     1001      127   575422 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/js_compiler/__init__.py
--rw-r--r--   0     1001      127     9973 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/js_compiler/test_javascript.py
--rw-r--r--   0     1001      127      808 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/js_compiler/test_postcss.py
--rw-r--r--   0     1001      127     2823 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/js_compiler/test_source_maps.py
--rw-r--r--   0     1001      127     1236 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/test_annotation_helpers.py
--rw-r--r--   0     1001      127     8602 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/test_app.py
--rw-r--r--   0     1001      127      734 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/test_cache.py
--rw-r--r--   0     1001      127     5281 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/test_cli.py
--rw-r--r--   0     1001      127      494 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/test_config.py
--rw-r--r--   0     1001      127     6571 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/test_controller.py
--rw-r--r--   0     1001      127     3239 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/test_cropper.py
--rw-r--r--   0     1001      127     1227 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/test_exceptions.py
--rw-r--r--   0     1001      127     1924 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/test_logging.py
--rw-r--r--   0     1001      127     8419 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/test_paths.py
--rw-r--r--   0     1001      127     2565 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/test_ssr.py
--rw-r--r--   0     1001      127     3177 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/__tests__/test_watch.py
--rw-r--r--   0     1001      127      397 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/actions/__init__.py
--rw-r--r--   0     1001      127    12321 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/actions/fields.py
--rw-r--r--   0     1001      127     6835 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/actions/passthrough.py
--rw-r--r--   0     1001      127    11635 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/actions/sideeffect.py
--rw-r--r--   0     1001      127     4352 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/annotation_helpers.py
--rw-r--r--   0     1001      127    18916 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/app.py
--rw-r--r--   0     1001      127     3216 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/cache.py
--rw-r--r--   0     1001      127    18059 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/cli.py
--rw-r--r--   0     1001      127    10826 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/client_builder/build_actions.py
--rw-r--r--   0     1001      127     3958 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/client_builder/build_links.py
--rw-r--r--   0     1001      127    11093 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/client_builder/build_schemas.py
--rw-r--r--   0     1001      127    28180 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/client_builder/builder.py
--rw-r--r--   0     1001      127    11312 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/client_builder/openapi.py
--rw-r--r--   0     1001      127     3253 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/client_builder/typescript.py
--rw-r--r--   0     1001      127     2424 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/config.py
--rw-r--r--   0     1001      127       40 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/constants.py
--rw-r--r--   0     1001      127    14854 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/controller.py
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/controllers/__init__.py
--rw-r--r--   0     1001      127     1216 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/controllers/exception_controller.py
--rw-r--r--   0     1001      127    10359 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/cropper.py
--rw-r--r--   0     1001      127      327 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/database/__init__.py
--rw-r--r--   0     1001      127     1866 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/database/cli.py
--rw-r--r--   0     1001      127     1822 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/database/config.py
--rw-r--r--   0     1001      127      133 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/database/dependencies/__init__.py
--rw-r--r--   0     1001      127     3188 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/database/dependencies/core.py
--rw-r--r--   0     1001      127     7969 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/database/sqlmodel.py
--rw-r--r--   0     1001      127     8737 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/database/validator.py
--rw-r--r--   0     1001      127      251 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/dependencies/__init__.py
--rw-r--r--   0     1001      127     5122 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/dependencies/base.py
--rw-r--r--   0     1001      127      116 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/dependencies/core/__init__.py
--rw-r--r--   0     1001      127     1069 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/dependencies/core/core.py
--rw-r--r--   0     1001      127     3317 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/exceptions.py
--rw-r--r--   0     1001      127     1188 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/io.py
--rw-r--r--   0     1001      127        1 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/js_compiler/__init__.py
--rw-r--r--   0     1001      127     1731 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/js_compiler/base.py
--rw-r--r--   0     1001      127      199 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/js_compiler/exceptions.py
--rw-r--r--   0     1001      127    15443 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/js_compiler/javascript.py
--rw-r--r--   0     1001      127     4163 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/js_compiler/postcss.py
--rw-r--r--   0     1001      127     5614 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/js_compiler/source_maps.py
--rw-r--r--   0     1001      127     2039 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/logging.py
--rw-r--r--   0     1001      127    12599 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/paths.py
--rw-r--r--   0     1001      127        0 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/py.typed
--rw-r--r--   0     1001      127     5816 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/render.py
--rw-r--r--   0     1001      127     3228 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/ssr.py
--rw-r--r--   0     1001      127      210 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/static/__init__.py
--rw-r--r--   0     1001      127     6299 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/static/api.ts
--rw-r--r--   0     1001      127     3976 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/static/live_reload.ts
--rw-r--r--   0     1001      127      323 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/static/ssr_polyfills.js
--rw-r--r--   0     1001      127     7261 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/test_utilities.py
--rw-r--r--   0     1001      127      213 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/views/__init__.py
--rw-r--r--   0     1001      127      432 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/views/core/exception/page.tsx
--rw-r--r--   0     1001      127      178 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/views/core/layout.tsx
--rw-r--r--   0     1001      127       59 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/views/core/main.css
--rw-r--r--   0     1001      127     1478 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/views/package-lock.json
--rw-r--r--   0     1001      127      257 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/views/package.json
--rw-r--r--   0     1001      127       83 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/views/postcss.config.js
--rw-r--r--   0     1001      127      162 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/views/tailwind.config.js
--rw-r--r--   0     1001      127     8378 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/watch.py
--rw-r--r--   0     1001      127     3087 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/watch_server.py
--rw-r--r--   0     1001      127      866 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/mountaineer/webservice.py
--rw-r--r--   0     1001      127   125089 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/poetry.lock
--rw-r--r--   0     1001      127   453080 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src/benches/fixtures/complex_sourcemap_mapping.txt
--rw-r--r--   0     1001      127   575422 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src/benches/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127      322 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src/benches/fixtures/ssr_polyfill_archive.js
--rw-r--r--   0     1001      127      899 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src/benches/lexers_benchmark.rs
--rw-r--r--   0     1001      127     1089 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src/benches/source_map_benchmark.rs
--rw-r--r--   0     1001      127     1595 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src/benches/ssr_benchmark.rs
--rw-r--r--   0     1001      127      499 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src/errors.rs
--rw-r--r--   0     1001      127     4648 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src/lexers.rs
--rw-r--r--   0     1001      127     8366 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src/lib.rs
--rw-r--r--   0     1001      127      680 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src/logging.rs
--rw-r--r--   0     1001      127    17549 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src/source_map.rs
--rw-r--r--   0     1001      127    15113 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src/ssr.rs
--rw-r--r--   0     1001      127     3998 2024-04-12 14:36:45.000000 mountaineer-0.4.1.dev2/src/timeout.rs
--rw-r--r--   0     1001      127    32093 2024-04-12 14:37:01.000000 mountaineer-0.4.1.dev2/Cargo.lock
--rw-r--r--   0     1001      127     1599 2024-04-12 14:36:58.000000 mountaineer-0.4.1.dev2/pyproject.toml
--rw-r--r--   0        0        0    15334 1970-01-01 00:00:00.000000 mountaineer-0.4.1.dev2/PKG-INFO
+-rw-r--r--   0     1001      127      269 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src_go/Cargo.toml
+-rw-r--r--   0     1001      127     1995 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src_go/build.rs
+-rw-r--r--   0     1001      127     5657 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src_go/go/js_build.go
+-rw-r--r--   0     1001      127      168 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src_go/go.mod
+-rw-r--r--   0     1001      127      376 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src_go/go.sum
+-rw-r--r--   0     1001      127     5750 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src_go/src/lib.rs
+-rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.4.1.dev3/Cargo.toml
+-rw-r--r--   0     1001      127      133 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/.git-blame-ignore-revs
+-rw-r--r--   0     1001      127      138 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/.gitattributes
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/.github/README_SCRIPTS.md
+-rw-r--r--   0     1001      127    14036 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/.github/poetry.lock
+-rw-r--r--   0     1001      127      767 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/.github/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/.github/scripts/__init__.py
+-rw-r--r--   0     1001      127     3032 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/.github/scripts/__tests__/test_update_version.py
+-rw-r--r--   0     1001      127     2181 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/.github/scripts/check_dependencies.py
+-rw-r--r--   0     1001      127     3382 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/.github/scripts/update_version.py
+-rw-r--r--   0     1001      127     1321 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/.github/workflows/publish_docs.yml
+-rw-r--r--   0     1001      127    19767 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      504 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/.github/workflows/validate.yml
+-rw-r--r--   0     1001      127     3404 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/.gitignore
+-rw-r--r--   0     1001      127     1750 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/Dockerfile
+-rw-r--r--   0     1001      127     1079 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/LICENSE
+-rw-r--r--   0     1001      127     4976 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/Makefile
+-rw-r--r--   0     1001      127    14891 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/README.md
+-rw-r--r--   0     1001      127      105 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/benchmarking/README.md
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/benchmarking/benchmarking/__init__.py
+-rw-r--r--   0     1001      127      425 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/benchmarking/benchmarking/simple_render.py
+-rw-r--r--   0     1001      127   127093 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/benchmarking/poetry.lock
+-rw-r--r--   0     1001      127      291 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/benchmarking/pyproject.toml
+-rw-r--r--   0     1001      127      850 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/README.md
+-rw-r--r--   0     1001      127        1 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/__init__.py
+-rw-r--r--   0     1001      127      775 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/app.py
+-rw-r--r--   0     1001      127      489 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/cli.py
+-rw-r--r--   0     1001      127      111 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/config.py
+-rw-r--r--   0     1001      127        1 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/controllers/__init__.py
+-rw-r--r--   0     1001      127     1433 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/controllers/complex.py
+-rw-r--r--   0     1001      127      581 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/controllers/detail.py
+-rw-r--r--   0     1001      127     1658 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/controllers/home.py
+-rw-r--r--   0     1001      127      559 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/controllers/stream.py
+-rw-r--r--   0     1001      127       77 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/main.py
+-rw-r--r--   0     1001      127      208 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/views/__init__.py
+-rw-r--r--   0     1001      127     2261 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/views/app/complex/page.tsx
+-rw-r--r--   0     1001      127      453 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127     2822 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       59 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/views/app/main.css
+-rw-r--r--   0     1001      127      708 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/views/app/stream/page.tsx
+-rw-r--r--   0     1001      127   125408 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/views/package-lock.json
+-rw-r--r--   0     1001      127      453 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/views/package.json
+-rw-r--r--   0     1001      127       83 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/views/postcss.config.js
+-rw-r--r--   0     1001      127      161 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/views/tailwind.config.js
+-rw-r--r--   0     1001      127   107805 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/poetry.lock
+-rw-r--r--   0     1001      127      724 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/ci_webapp/pyproject.toml
+-rw-r--r--   0     1001      127     1593 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/README.md
+-rw-r--r--   0     1001      127        1 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
+-rw-r--r--   0     1001      127     1055 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
+-rw-r--r--   0     1001      127     7904 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
+-rw-r--r--   0     1001      127      292 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      816 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
+-rw-r--r--   0     1001      127     4277 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/builder.py
+-rw-r--r--   0     1001      127     4656 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/cli.py
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
+-rw-r--r--   0     1001      127     1383 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/environments/base.py
+-rw-r--r--   0     1001      127     4591 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
+-rw-r--r--   0     1001      127     1832 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/environments/venv.py
+-rw-r--r--   0     1001      127     1336 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/external.py
+-rw-r--r--   0     1001      127     1925 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/generation.py
+-rw-r--r--   0     1001      127      327 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/io.py
+-rw-r--r--   0     1001      127       30 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
+-rw-r--r--   0     1001      127      212 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
+-rw-r--r--   0     1001      127      190 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
+-rw-r--r--   0     1001      127      137 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
+-rw-r--r--   0     1001      127      109 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
+-rw-r--r--   0     1001      127      170 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.env
+-rw-r--r--   0     1001      127     3373 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
+-rw-r--r--   0     1001      127      645 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
+-rw-r--r--   0     1001      127       17 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
+-rw-r--r--   0     1001      127      767 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
+-rw-r--r--   0     1001      127      947 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
+-rw-r--r--   0     1001      127      282 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
+-rw-r--r--   0     1001      127      227 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
+-rw-r--r--   0     1001      127     1702 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
+-rw-r--r--   0     1001      127     1124 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
+-rw-r--r--   0     1001      127       84 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
+-rw-r--r--   0     1001      127      157 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
+-rw-r--r--   0     1001      127      208 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
+-rw-r--r--   0     1001      127     1219 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127      995 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       95 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
+-rw-r--r--   0     1001      127      524 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
+-rw-r--r--   0     1001      127      117 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
+-rw-r--r--   0     1001      127      195 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
+-rw-r--r--   0     1001      127      332 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
+-rw-r--r--   0     1001      127     1493 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
+-rw-r--r--   0     1001      127    61104 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/poetry.lock
+-rw-r--r--   0     1001      127     1214 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/create_mountaineer_app/pyproject.toml
+-rw-r--r--   0     1001      127       30 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/.zed/settings.json
+-rw-r--r--   0     1001      127      107 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/README.md
+-rw-r--r--   0     1001      127       15 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/CNAME
+-rw-r--r--   0     1001      127      310 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/actions.md
+-rw-r--r--   0     1001      127      454 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/api_exception.md
+-rw-r--r--   0     1001      127       99 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/app-controller.md
+-rw-r--r--   0     1001      127      281 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/build_plugins/base.md
+-rw-r--r--   0     1001      127       57 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/build_plugins/javascript.md
+-rw-r--r--   0     1001      127       62 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/build_plugins/postcss.md
+-rw-r--r--   0     1001      127      411 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/cli.md
+-rw-r--r--   0     1001      127      376 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/config.md
+-rw-r--r--   0     1001      127       61 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/controller.md
+-rw-r--r--   0     1001      127       67 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/core_dependencies.md
+-rw-r--r--   0     1001      127       66 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/database/config.md
+-rw-r--r--   0     1001      127       71 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/database/dependencies.md
+-rw-r--r--   0     1001      127       80 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/logging.md
+-rw-r--r--   0     1001      127      479 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/render.md
+-rw-r--r--   0     1001      127      365 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/ssr.md
+-rw-r--r--   0     1001      127      299 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/api/watch_server.md
+-rw-r--r--   0     1001      127     9375 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/client_actions.md
+-rw-r--r--   0     1001      127      753 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/cma.md
+-rw-r--r--   0     1001      127     3021 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/database.md
+-rw-r--r--   0     1001      127     4677 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/deploy.md
+-rw-r--r--   0     1001      127     7698 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/error_handling.md
+-rw-r--r--   0     1001      127     1081 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/index.md
+-rw-r--r--   0     1001      127     1541 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/internal/core_library.md
+-rw-r--r--   0     1001      127     2156 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/links.md
+-rw-r--r--   0     1001      127   365251 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/media/final_todo_list.png
+-rw-r--r--   0     1001      127   148261 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/media/ide_typehints.png
+-rw-r--r--   0     1001      127   545494 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/media/network_debug.png
+-rw-r--r--   0     1001      127   346903 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/media/server_side_rendering.png
+-rw-r--r--   0     1001      127     2263 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/metadata.md
+-rw-r--r--   0     1001      127     2347 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/postcss.md
+-rw-r--r--   0     1001      127    12265 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/quickstart.md
+-rw-r--r--   0     1001      127     4875 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/static_analysis.md
+-rw-r--r--   0     1001      127     2490 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/structure.md
+-rw-r--r--   0     1001      127     1219 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/stylesheets/extra.css
+-rw-r--r--   0     1001      127     4080 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/docs/views.md
+-rw-r--r--   0     1001      127     1823 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/mkdocs.yml
+-rw-r--r--   0     1001      127      109 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/overrides/partials/footer.html
+-rw-r--r--   0     1001      127   156250 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/poetry.lock
+-rw-r--r--   0     1001      127      479 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/docs_website/pyproject.toml
+-rw-r--r--   0     1001      127   675789 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/media/header.png
+-rw-r--r--   0     1001      127      954 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/actions/__init__.py
+-rw-r--r--   0     1001      127     7884 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/actions/test_fields.py
+-rw-r--r--   0     1001      127     9707 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/actions/test_passthrough.py
+-rw-r--r--   0     1001      127     9074 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/actions/test_sideeffect.py
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/client_builder/__init__.py
+-rw-r--r--   0     1001      127    14334 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/client_builder/test_build_actions.py
+-rw-r--r--   0     1001      127     4816 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/client_builder/test_build_links.py
+-rw-r--r--   0     1001      127    10097 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/client_builder/test_build_schemas.py
+-rw-r--r--   0     1001      127     5001 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/client_builder/test_builder.py
+-rw-r--r--   0     1001      127     4153 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/client_builder/test_typescript.py
+-rw-r--r--   0     1001      127      319 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/common.py
+-rw-r--r--   0     1001      127      497 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/conftest.py
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/database/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127      208 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/database/dependencies/conftest.py
+-rw-r--r--   0     1001      127      801 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/database/dependencies/test_core.py
+-rw-r--r--   0     1001      127      627 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/database/test_config.py
+-rw-r--r--   0     1001      127      616 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/database/test_sqlmodel.py
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/dependencies/__init__.py
+-rw-r--r--   0     1001      127     2567 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/dependencies/test_base.py
+-rw-r--r--   0     1001      127      211 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/fixtures/__init__.py
+-rw-r--r--   0     1001      127   571338 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127  1638568 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
+-rw-r--r--   0     1001      127   575422 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     9973 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/js_compiler/test_javascript.py
+-rw-r--r--   0     1001      127      808 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/js_compiler/test_postcss.py
+-rw-r--r--   0     1001      127     2823 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/js_compiler/test_source_maps.py
+-rw-r--r--   0     1001      127     1236 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/test_annotation_helpers.py
+-rw-r--r--   0     1001      127     8602 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/test_app.py
+-rw-r--r--   0     1001      127      734 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/test_cache.py
+-rw-r--r--   0     1001      127     5281 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      494 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/test_config.py
+-rw-r--r--   0     1001      127     6571 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/test_controller.py
+-rw-r--r--   0     1001      127     3239 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/test_cropper.py
+-rw-r--r--   0     1001      127     1227 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/test_exceptions.py
+-rw-r--r--   0     1001      127     1924 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/test_logging.py
+-rw-r--r--   0     1001      127     8419 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/test_paths.py
+-rw-r--r--   0     1001      127     2565 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/test_ssr.py
+-rw-r--r--   0     1001      127     3177 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/__tests__/test_watch.py
+-rw-r--r--   0     1001      127      397 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/actions/__init__.py
+-rw-r--r--   0     1001      127    12321 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/actions/fields.py
+-rw-r--r--   0     1001      127     6835 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/actions/passthrough.py
+-rw-r--r--   0     1001      127    11635 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/actions/sideeffect.py
+-rw-r--r--   0     1001      127     4352 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/annotation_helpers.py
+-rw-r--r--   0     1001      127    18916 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/app.py
+-rw-r--r--   0     1001      127     3216 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/cache.py
+-rw-r--r--   0     1001      127    18059 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/cli.py
+-rw-r--r--   0     1001      127    11390 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/client_builder/build_actions.py
+-rw-r--r--   0     1001      127     4002 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/client_builder/build_links.py
+-rw-r--r--   0     1001      127    10172 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/client_builder/build_schemas.py
+-rw-r--r--   0     1001      127    28180 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/client_builder/builder.py
+-rw-r--r--   0     1001      127    11199 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/client_builder/openapi.py
+-rw-r--r--   0     1001      127     5070 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/client_builder/typescript.py
+-rw-r--r--   0     1001      127     2424 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/config.py
+-rw-r--r--   0     1001      127       40 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/constants.py
+-rw-r--r--   0     1001      127    14854 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/controller.py
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/controllers/__init__.py
+-rw-r--r--   0     1001      127     1216 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/controllers/exception_controller.py
+-rw-r--r--   0     1001      127    10359 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/cropper.py
+-rw-r--r--   0     1001      127      327 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/database/__init__.py
+-rw-r--r--   0     1001      127     1866 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/database/cli.py
+-rw-r--r--   0     1001      127     1822 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/database/config.py
+-rw-r--r--   0     1001      127      133 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127     3188 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/database/dependencies/core.py
+-rw-r--r--   0     1001      127     7969 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/database/sqlmodel.py
+-rw-r--r--   0     1001      127     8737 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/database/validator.py
+-rw-r--r--   0     1001      127      251 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/dependencies/__init__.py
+-rw-r--r--   0     1001      127     5122 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/dependencies/base.py
+-rw-r--r--   0     1001      127      116 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/dependencies/core/__init__.py
+-rw-r--r--   0     1001      127     1069 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/dependencies/core/core.py
+-rw-r--r--   0     1001      127     3317 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/exceptions.py
+-rw-r--r--   0     1001      127     1188 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/io.py
+-rw-r--r--   0     1001      127        1 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     1731 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/js_compiler/base.py
+-rw-r--r--   0     1001      127      199 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/js_compiler/exceptions.py
+-rw-r--r--   0     1001      127    15443 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/js_compiler/javascript.py
+-rw-r--r--   0     1001      127     4163 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/js_compiler/postcss.py
+-rw-r--r--   0     1001      127     5614 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/js_compiler/source_maps.py
+-rw-r--r--   0     1001      127     2039 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/logging.py
+-rw-r--r--   0     1001      127    12599 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/paths.py
+-rw-r--r--   0     1001      127        0 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/py.typed
+-rw-r--r--   0     1001      127     5816 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/render.py
+-rw-r--r--   0     1001      127     3228 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/ssr.py
+-rw-r--r--   0     1001      127      210 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/static/__init__.py
+-rw-r--r--   0     1001      127     6299 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/static/api.ts
+-rw-r--r--   0     1001      127     3976 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/static/live_reload.ts
+-rw-r--r--   0     1001      127      323 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/static/ssr_polyfills.js
+-rw-r--r--   0     1001      127     7261 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/test_utilities.py
+-rw-r--r--   0     1001      127      213 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/views/__init__.py
+-rw-r--r--   0     1001      127      432 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/views/core/exception/page.tsx
+-rw-r--r--   0     1001      127      178 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/views/core/layout.tsx
+-rw-r--r--   0     1001      127       59 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/views/core/main.css
+-rw-r--r--   0     1001      127     1478 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/views/package-lock.json
+-rw-r--r--   0     1001      127      257 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/views/package.json
+-rw-r--r--   0     1001      127       83 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/views/postcss.config.js
+-rw-r--r--   0     1001      127      162 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/views/tailwind.config.js
+-rw-r--r--   0     1001      127     8378 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/watch.py
+-rw-r--r--   0     1001      127     3087 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/watch_server.py
+-rw-r--r--   0     1001      127      866 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/mountaineer/webservice.py
+-rw-r--r--   0     1001      127   125089 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/poetry.lock
+-rw-r--r--   0     1001      127   453080 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src/benches/fixtures/complex_sourcemap_mapping.txt
+-rw-r--r--   0     1001      127   575422 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src/benches/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127      322 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src/benches/fixtures/ssr_polyfill_archive.js
+-rw-r--r--   0     1001      127      899 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src/benches/lexers_benchmark.rs
+-rw-r--r--   0     1001      127     1089 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src/benches/source_map_benchmark.rs
+-rw-r--r--   0     1001      127     1595 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src/benches/ssr_benchmark.rs
+-rw-r--r--   0     1001      127      499 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src/errors.rs
+-rw-r--r--   0     1001      127     4648 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src/lexers.rs
+-rw-r--r--   0     1001      127     8366 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src/lib.rs
+-rw-r--r--   0     1001      127      680 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src/logging.rs
+-rw-r--r--   0     1001      127    17549 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src/source_map.rs
+-rw-r--r--   0     1001      127    15113 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src/ssr.rs
+-rw-r--r--   0     1001      127     3998 2024-04-16 23:40:48.000000 mountaineer-0.4.1.dev3/src/timeout.rs
+-rw-r--r--   0     1001      127    32093 2024-04-16 23:41:06.000000 mountaineer-0.4.1.dev3/Cargo.lock
+-rw-r--r--   0     1001      127     1599 2024-04-16 23:41:03.000000 mountaineer-0.4.1.dev3/pyproject.toml
+-rw-r--r--   0        0        0    15334 1970-01-01 00:00:00.000000 mountaineer-0.4.1.dev3/PKG-INFO
```

### Comparing `mountaineer-0.4.1.dev2/src_go/build.rs` & `mountaineer-0.4.1.dev3/src_go/build.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/src_go/go/js_build.go` & `mountaineer-0.4.1.dev3/src_go/go/js_build.go`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/src_go/src/lib.rs` & `mountaineer-0.4.1.dev3/src_go/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/Cargo.toml` & `mountaineer-0.4.1.dev3/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [[bench]]
 path = "src/benches/lexers_benchmark.rs"
 name = "lexers_benchmark"
 harness = false
 
 [package]
 name = "mountaineer"
-version = "0.4.1-dev2"
+version = "0.4.1-dev3"
 edition = "2021"
 
 [dependencies]
 v8 = "0.89.0"
 deno_core_icudata = "0.73.0"
 lazy_static = "1.4.0"
 serde_json = "1.0"
```

### Comparing `mountaineer-0.4.1.dev2/.github/poetry.lock` & `mountaineer-0.4.1.dev3/.github/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/.github/pyproject.toml` & `mountaineer-0.4.1.dev3/.github/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/.github/scripts/__tests__/test_update_version.py` & `mountaineer-0.4.1.dev3/.github/scripts/__tests__/test_update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/.github/scripts/check_dependencies.py` & `mountaineer-0.4.1.dev3/.github/scripts/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/.github/scripts/update_version.py` & `mountaineer-0.4.1.dev3/.github/scripts/update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/.github/workflows/publish_docs.yml` & `mountaineer-0.4.1.dev3/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/.github/workflows/test.yml` & `mountaineer-0.4.1.dev3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/.gitignore` & `mountaineer-0.4.1.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/Dockerfile` & `mountaineer-0.4.1.dev3/Dockerfile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/LICENSE` & `mountaineer-0.4.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/Makefile` & `mountaineer-0.4.1.dev3/Makefile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/README.md` & `mountaineer-0.4.1.dev3/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/benchmarking/poetry.lock` & `mountaineer-0.4.1.dev3/benchmarking/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/ci_webapp/README.md` & `mountaineer-0.4.1.dev3/ci_webapp/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/app.py` & `mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/controllers/complex.py` & `mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/controllers/complex.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/controllers/detail.py` & `mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/controllers/home.py` & `mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/controllers/stream.py` & `mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/controllers/stream.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/views/app/complex/page.tsx` & `mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/views/app/complex/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/views/app/home/page.tsx` & `mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/views/app/stream/page.tsx` & `mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/views/app/stream/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/ci_webapp/ci_webapp/views/package-lock.json` & `mountaineer-0.4.1.dev3/ci_webapp/ci_webapp/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/ci_webapp/poetry.lock` & `mountaineer-0.4.1.dev3/ci_webapp/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/ci_webapp/pyproject.toml` & `mountaineer-0.4.1.dev3/ci_webapp/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/README.md` & `mountaineer-0.4.1.dev3/create_mountaineer_app/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/common.py` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/common.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/builder.py` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/cli.py` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/environments/base.py` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/environments/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/environments/poetry.py` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/environments/poetry.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/environments/venv.py` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/environments/venv.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/external.py` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/external.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/generation.py` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/README.md` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml` & `mountaineer-0.4.1.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/poetry.lock` & `mountaineer-0.4.1.dev3/create_mountaineer_app/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/create_mountaineer_app/pyproject.toml` & `mountaineer-0.4.1.dev3/create_mountaineer_app/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/client_actions.md` & `mountaineer-0.4.1.dev3/docs_website/docs/client_actions.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/cma.md` & `mountaineer-0.4.1.dev3/docs_website/docs/cma.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/database.md` & `mountaineer-0.4.1.dev3/docs_website/docs/database.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/deploy.md` & `mountaineer-0.4.1.dev3/docs_website/docs/deploy.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/error_handling.md` & `mountaineer-0.4.1.dev3/docs_website/docs/error_handling.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/index.md` & `mountaineer-0.4.1.dev3/docs_website/docs/index.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/internal/core_library.md` & `mountaineer-0.4.1.dev3/docs_website/docs/internal/core_library.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/links.md` & `mountaineer-0.4.1.dev3/docs_website/docs/links.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/media/final_todo_list.png` & `mountaineer-0.4.1.dev3/docs_website/docs/media/final_todo_list.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/media/ide_typehints.png` & `mountaineer-0.4.1.dev3/docs_website/docs/media/ide_typehints.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/media/network_debug.png` & `mountaineer-0.4.1.dev3/docs_website/docs/media/network_debug.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/media/server_side_rendering.png` & `mountaineer-0.4.1.dev3/docs_website/docs/media/server_side_rendering.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/metadata.md` & `mountaineer-0.4.1.dev3/docs_website/docs/metadata.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/postcss.md` & `mountaineer-0.4.1.dev3/docs_website/docs/postcss.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/quickstart.md` & `mountaineer-0.4.1.dev3/docs_website/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/static_analysis.md` & `mountaineer-0.4.1.dev3/docs_website/docs/static_analysis.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/structure.md` & `mountaineer-0.4.1.dev3/docs_website/docs/structure.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/stylesheets/extra.css` & `mountaineer-0.4.1.dev3/docs_website/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/docs/views.md` & `mountaineer-0.4.1.dev3/docs_website/docs/views.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/mkdocs.yml` & `mountaineer-0.4.1.dev3/docs_website/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/docs_website/poetry.lock` & `mountaineer-0.4.1.dev3/docs_website/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/media/header.png` & `mountaineer-0.4.1.dev3/media/header.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__init__.py` & `mountaineer-0.4.1.dev3/mountaineer/__init__.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/actions/test_fields.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/actions/test_fields.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/actions/test_passthrough.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/actions/test_passthrough.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/actions/test_sideeffect.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/actions/test_sideeffect.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/client_builder/test_build_actions.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/client_builder/test_build_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+from datetime import datetime
 from re import sub as re_sub
+from uuid import UUID
 
 import pytest
 from fastapi import APIRouter
 from fastapi.openapi.utils import get_openapi
 from pydantic import BaseModel
 
 from mountaineer.client_builder.build_actions import OpenAPIToTypescriptActionConverter
@@ -121,14 +123,45 @@
                 """
             ),
             [
                 "ExampleModel",
                 "ExampleResponseModel",
             ],
         ),
+        # No request body parameter
+        (
+            "my_method_fn",
+            "/testing/url",
+            ActionDefinition(
+                action_type=ActionType.POST,
+                summary="",
+                operationId="",
+                requestBody=None,
+                responses={
+                    "200": EXAMPLE_RESPONSE_200,
+                    "422": EXAMPLE_RESPONSE_400,
+                },
+            ),
+            (
+                """
+                export const my_method_fn = (): Promise<ExampleResponseModel> => {
+                    return __request({
+                        'method': 'POST',
+                        'url': '/testing/url',
+                        'errors': {
+                            422: HTTPValidationErrorException
+                        }
+                    });
+                }
+                """
+            ),
+            [
+                "ExampleResponseModel",
+            ],
+        ),
         # Path and query parameters
         (
             "my_method_fn",
             "/testing/{item_id}",
             ActionDefinition(
                 action_type=ActionType.POST,
                 summary="",
@@ -359,7 +392,34 @@
     expected_function: str,
     expected_imports: list[str],
 ):
     builder = OpenAPIToTypescriptActionConverter()
     built_function, build_imports = builder.build_action(url, definition, method_name)
     assert re_sub(r"\s+", "", built_function) == re_sub(r"\s+", "", expected_function)
     assert set(build_imports) == set(expected_imports)
+
+
+AnyType = None | bool | str | int | datetime | UUID
+DictParamItem = dict[str, AnyType]
+
+
+def test_build_invalid_action_api():
+    """
+    Ensure that we throw an error if the user has provided a schema payload
+    that is technically valid, but doesn't allow typehinting with pydantic. All non-raw
+    JSON requests should be Pydantic methods.
+
+    https://github.com/piercefreeman/mountaineer/issues/94
+
+    """
+
+    def fn1(payload: DictParamItem, item_id: str, other_id: str) -> None:
+        pass
+
+    router = APIRouter()
+    router.post("/fn1")(fn1)
+
+    builder = OpenAPIToTypescriptActionConverter()
+    openapi_spec = get_openapi(title="", version="", routes=router.routes)
+
+    with pytest.raises(ValueError):
+        builder.convert(openapi_spec)
```

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/client_builder/test_build_links.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/client_builder/test_build_links.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from enum import StrEnum
 from re import sub as re_sub
 from typing import Callable
+from uuid import UUID
 
 import pytest
 from fastapi import APIRouter
 from fastapi.openapi.utils import get_openapi
 
 from mountaineer.client_builder.build_links import OpenAPIToTypescriptLinkConverter
 
@@ -16,14 +18,28 @@
     pass
 
 
 def view_endpoint_query_params(query_a: str, query_b: int | None = None):
     pass
 
 
+class RouteType(StrEnum):
+    ROUTE_A = "route_a"
+    ROUTE_B = "route_b"
+
+
+def enum_view_url(model_type: RouteType, model_id: UUID):
+    """
+    Model view paths like /{model_type}/{model_id} where we want a flexible
+    string to be captured in the model_type path.
+
+    """
+    pass
+
+
 @pytest.mark.parametrize(
     "url, endpoint, expected_link",
     [
         # Regular view endpoint, no render params
         (
             "/regular/",
             view_endpoint_regular,
@@ -92,14 +108,43 @@
                     return __getLink({
                         rawUrl: url,
                         queryParameters,
                         pathParameters
                     });
                 };
                 """
+            ),
+        ),
+        # Path with enum path variables - we should typehint explicitly
+        # as the enum based values
+        (
+            "/enum_view/{model_type}/{model_id}",
+            enum_view_url,
+            (
+                """
+                export const getLink = ({
+                    model_type,
+                    model_id
+                }:{
+                    model_type: 'route_a' | 'route_b',
+                    model_id: string
+                }) => {
+                    const url = `/enum_view/{model_type}/{model_id}`;
+                    const queryParameters: Record<string,any> = {};
+                    const pathParameters: Record<string,any> = {
+                        model_type,
+                        model_id
+                    };
+                    return __getLink({
+                        rawUrl: url,
+                        queryParameters,
+                        pathParameters
+                    });
+                };
+                """
             ),
         ),
     ],
 )
 def test_convert(url: str, endpoint: Callable, expected_link: str):
     # Each function needs a response model because we expect that all @sideeffect
     # and @passthrough functions will have an automatically defined response model
```

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/client_builder/test_build_schemas.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/client_builder/test_build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/client_builder/test_builder.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/client_builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/client_builder/test_typescript.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/client_builder/test_typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/database/dependencies/test_core.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/database/dependencies/test_core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/database/test_config.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/database/test_config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/database/test_sqlmodel.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/database/test_sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/dependencies/test_base.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/dependencies/test_base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/fixtures/home_controller_source_map.js.map` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/fixtures/home_controller_source_map.js.map`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/js_compiler/test_javascript.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/js_compiler/test_javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/js_compiler/test_postcss.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/js_compiler/test_postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/js_compiler/test_source_maps.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/js_compiler/test_source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/test_annotation_helpers.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/test_annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/test_app.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/test_app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/test_cache.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/test_cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/test_cli.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/test_cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/test_controller.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/test_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/test_cropper.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/test_cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/test_exceptions.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/test_logging.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/test_logging.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/test_paths.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/test_paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/test_ssr.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/test_ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/__tests__/test_watch.py` & `mountaineer-0.4.1.dev3/mountaineer/__tests__/test_watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/actions/fields.py` & `mountaineer-0.4.1.dev3/mountaineer/actions/fields.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/actions/passthrough.py` & `mountaineer-0.4.1.dev3/mountaineer/actions/passthrough.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/actions/sideeffect.py` & `mountaineer-0.4.1.dev3/mountaineer/actions/sideeffect.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/annotation_helpers.py` & `mountaineer-0.4.1.dev3/mountaineer/annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/app.py` & `mountaineer-0.4.1.dev3/mountaineer/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/cache.py` & `mountaineer-0.4.1.dev3/mountaineer/cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/cli.py` & `mountaineer-0.4.1.dev3/mountaineer/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/client_builder/build_actions.py` & `mountaineer-0.4.1.dev3/mountaineer/client_builder/build_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,20 +200,24 @@
             status_int = int(status_code)
             if self.status_code_is_valid(status_int):
                 # OK response, we can specify the expected response type
                 # Multiple OK responses for a single action is unusual, but again we support it
                 if not action.is_raw_response:
                     response_types.append(
                         self.get_typescript_name_from_content_definition(
-                            response_definition.content_schema
+                            response_definition.content_schema,
+                            url=url,
+                            status_code=status_int,
                         )
                     )
             else:
                 error_typehint = self.get_typescript_name_from_content_definition(
-                    response_definition.content_schema
+                    response_definition.content_schema,
+                    url=url,
+                    status_code=status_int,
                 )
                 common_params["errors"][status_int] = TSLiteral(
                     # Provide a mapping to the error class
                     self.get_exception_class_name(error_typehint)
                 )
 
         # Remove the optional keys that don't have any values
@@ -249,19 +253,26 @@
                 method_names.append(f"{base_method_name}_{action.action_type.lower()}")
         else:
             method_names.append(base_method_name)
 
         return method_names
 
     def get_typescript_name_from_content_definition(
-        self, definition: ContentDefinition
+        self,
+        definition: ContentDefinition,
+        # Url and status are provided for more context about where the error
+        # is being thrown. Can pass None if not available.
+        url: str | None = None,
+        status_code: int | None = None,
     ):
         if not definition.schema_ref.ref:
             raise ValueError(
-                f"Content definition {definition} does not have a schema reference"
+                f"Content definition {definition} does not have a schema reference.\n"
+                f"Double check your action definition for {url} with response code {status_code}.\n"
+                "Are you typehinting your response with a Pydantic BaseModel?"
             )
         return definition.schema_ref.ref.split("/")[-1]
 
     def status_code_is_valid(self, status_code: int):
         return status_code >= 200 and status_code < 300
 
     def get_exception_class_name(self, exception_typehint: str):
```

### Comparing `mountaineer-0.4.1.dev2/mountaineer/client_builder/build_links.py` & `mountaineer-0.4.1.dev3/mountaineer/client_builder/build_links.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,17 @@
             # We only support query and path parameters
             if parameter.in_location not in {
                 ParameterLocationType.QUERY,
                 ParameterLocationType.PATH,
             }:
                 continue
 
-            typehint_key, typehint_value = get_typehint_for_parameter(parameter)
+            typehint_key, typehint_value = get_typehint_for_parameter(
+                parameter, openapi_spec
+            )
             input_parameters[TSLiteral(parameter.name)] = TSLiteral(parameter.name)
             typehint_parameters[typehint_key] = typehint_value
 
             if parameter.in_location == ParameterLocationType.QUERY:
                 query_parameters[TSLiteral(parameter.name)] = TSLiteral(parameter.name)
             elif parameter.in_location == ParameterLocationType.PATH:
                 path_parameters[TSLiteral(parameter.name)] = TSLiteral(parameter.name)
```

### Comparing `mountaineer-0.4.1.dev2/mountaineer/client_builder/build_schemas.py` & `mountaineer-0.4.1.dev3/mountaineer/client_builder/build_schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 Generator for TypeScript interfaces from OpenAPI specifications.
 """
 from typing import Any, Dict, Iterator, Type, get_args, get_origin
 
 from inflection import camelize
 from pydantic import BaseModel, create_model
 
-from mountaineer.annotation_helpers import get_value_by_alias, yield_all_subtypes
+from mountaineer.annotation_helpers import yield_all_subtypes
 from mountaineer.client_builder.openapi import (
     EmptyAPIProperty,
     OpenAPIProperty,
     OpenAPISchema,
     OpenAPISchemaType,
+    resolve_ref,
 )
 from mountaineer.client_builder.typescript import (
     TSLiteral,
     map_openapi_type_to_ts,
     python_payload_to_typescript,
 )
 from mountaineer.logging import LOGGER
@@ -99,49 +100,27 @@
 
             if (
                 property.variable_type == OpenAPISchemaType.OBJECT
                 or property.enum is not None
             ):
                 yield property
             if property.ref is not None:
-                yield from walk_models(self.resolve_ref(property.ref, base))
+                yield from walk_models(resolve_ref(property.ref, base))
             if property.items:
                 yield from walk_models(property.items)
             if property.anyOf:
                 for prop in property.anyOf:
                     yield from walk_models(prop)
             for prop in property.properties.values():
                 yield from walk_models(prop)
             if property.additionalProperties:
                 yield from walk_models(property.additionalProperties)
 
         return list(set(walk_models(base)))
 
-    def resolve_ref(self, ref: str, base: BaseModel) -> OpenAPIProperty:
-        """
-        Resolve a $ref that points to a propery-compliant schema in the same document. If this
-        ref points somewhere else in the document (that is valid but not a data model) than we
-        raise a ValueError.
-
-        """
-        current_obj = base
-        for part in ref.split("/"):
-            if part == "#":
-                current_obj = base
-            else:
-                try:
-                    current_obj = get_value_by_alias(current_obj, part)
-                except AttributeError as e:
-                    raise AttributeError(
-                        f"Invalid $ref, couldn't resolve path: {ref}"
-                    ) from e
-        if not isinstance(current_obj, OpenAPIProperty):
-            raise ValueError(f"Resolved $ref is not a valid OpenAPIProperty: {ref}")
-        return current_obj
-
     def convert_schema_to_interface(
         self,
         model: OpenAPIProperty,
         base: BaseModel,
         defaults_are_required: bool,
         all_fields_required: bool,
     ):
@@ -184,15 +163,15 @@
 
                 array_types: list[str] = (
                     sorted(set(walk_array_types(prop.items))) if prop.items else ["any"]
                 )
                 yield f"Array<{' | '.join(array_types)}>"
             elif prop.ref:
                 yield self.get_typescript_interface_name(
-                    self.resolve_ref(prop.ref, base=base)
+                    resolve_ref(prop.ref, base=base)
                 )
             elif prop.items:
                 yield from walk_array_types(prop.items)
             elif prop.anyOf:
                 for sub_prop in prop.anyOf:
                     yield from walk_array_types(sub_prop)
             elif prop.additionalProperties:
```

### Comparing `mountaineer-0.4.1.dev2/mountaineer/client_builder/builder.py` & `mountaineer-0.4.1.dev3/mountaineer/client_builder/builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/client_builder/openapi.py` & `mountaineer-0.4.1.dev3/mountaineer/client_builder/openapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 from enum import StrEnum
 from typing import Any, Optional, Union
 
 from pydantic import BaseModel, ConfigDict, Field, model_validator
 
+from mountaineer.annotation_helpers import get_value_by_alias
+
 #
 # Enum definitions
 #
 
 
 class OpenAPISchemaType(StrEnum):
     OBJECT = "object"
@@ -320,37 +322,28 @@
 
 
 #
 # Helper methods
 #
 
 
-def get_types_from_parameters(schema: OpenAPIProperty | EmptyAPIProperty):
+def resolve_ref(ref: str, base: BaseModel) -> OpenAPIProperty:
     """
-    Handle potentially complex types from the parameter schema, like the case
-    of optional fields.
+    Resolve a $ref that points to a propery-compliant schema in the same document. If this
+    ref points somewhere else in the document (that is valid but not a data model) than we
+    raise a ValueError.
 
     """
-    if isinstance(schema, EmptyAPIProperty):
-        return "any"
-
-    # Recursively gather all of the types that might be nested
-    if schema.variable_type:
-        yield schema.variable_type
-
-    for property in schema.properties.values():
-        yield from get_types_from_parameters(property)
-
-    if schema.additionalProperties:
-        yield from get_types_from_parameters(schema.additionalProperties)
-
-    if schema.items:
-        yield from get_types_from_parameters(schema.items)
-
-    if schema.anyOf:
-        for one_of in schema.anyOf:
-            yield from get_types_from_parameters(one_of)
-
-    # We don't expect $ref values in the URL schema, if we do then the parsing
-    # is likely incorrect
-    if schema.ref:
-        raise ValueError(f"Unexpected $ref in URL schema: {schema.ref}")
+    current_obj = base
+    for part in ref.split("/"):
+        if part == "#":
+            current_obj = base
+        else:
+            try:
+                current_obj = get_value_by_alias(current_obj, part)
+            except AttributeError as e:
+                raise AttributeError(
+                    f"Invalid $ref, couldn't resolve path: {ref}"
+                ) from e
+    if not isinstance(current_obj, OpenAPIProperty):
+        raise ValueError(f"Resolved $ref is not a valid OpenAPIProperty: {ref}")
+    return current_obj
```

### Comparing `mountaineer-0.4.1.dev2/mountaineer/config.py` & `mountaineer-0.4.1.dev3/mountaineer/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/controller.py` & `mountaineer-0.4.1.dev3/mountaineer/controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/controllers/exception_controller.py` & `mountaineer-0.4.1.dev3/mountaineer/controllers/exception_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/cropper.py` & `mountaineer-0.4.1.dev3/mountaineer/cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/database/cli.py` & `mountaineer-0.4.1.dev3/mountaineer/database/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/database/config.py` & `mountaineer-0.4.1.dev3/mountaineer/database/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/database/dependencies/core.py` & `mountaineer-0.4.1.dev3/mountaineer/database/dependencies/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/database/sqlmodel.py` & `mountaineer-0.4.1.dev3/mountaineer/database/sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/database/validator.py` & `mountaineer-0.4.1.dev3/mountaineer/database/validator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/dependencies/base.py` & `mountaineer-0.4.1.dev3/mountaineer/dependencies/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/dependencies/core/core.py` & `mountaineer-0.4.1.dev3/mountaineer/dependencies/core/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/exceptions.py` & `mountaineer-0.4.1.dev3/mountaineer/exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/io.py` & `mountaineer-0.4.1.dev3/mountaineer/io.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/js_compiler/base.py` & `mountaineer-0.4.1.dev3/mountaineer/js_compiler/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/js_compiler/javascript.py` & `mountaineer-0.4.1.dev3/mountaineer/js_compiler/javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/js_compiler/postcss.py` & `mountaineer-0.4.1.dev3/mountaineer/js_compiler/postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/js_compiler/source_maps.py` & `mountaineer-0.4.1.dev3/mountaineer/js_compiler/source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/logging.py` & `mountaineer-0.4.1.dev3/mountaineer/logging.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/paths.py` & `mountaineer-0.4.1.dev3/mountaineer/paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/render.py` & `mountaineer-0.4.1.dev3/mountaineer/render.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/ssr.py` & `mountaineer-0.4.1.dev3/mountaineer/ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/static/api.ts` & `mountaineer-0.4.1.dev3/mountaineer/static/api.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/static/live_reload.ts` & `mountaineer-0.4.1.dev3/mountaineer/static/live_reload.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/test_utilities.py` & `mountaineer-0.4.1.dev3/mountaineer/test_utilities.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/views/package-lock.json` & `mountaineer-0.4.1.dev3/mountaineer/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/watch.py` & `mountaineer-0.4.1.dev3/mountaineer/watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/watch_server.py` & `mountaineer-0.4.1.dev3/mountaineer/watch_server.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/mountaineer/webservice.py` & `mountaineer-0.4.1.dev3/mountaineer/webservice.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/poetry.lock` & `mountaineer-0.4.1.dev3/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/src/benches/fixtures/complex_sourcemap_mapping.txt` & `mountaineer-0.4.1.dev3/src/benches/fixtures/complex_sourcemap_mapping.txt`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/src/benches/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.4.1.dev3/src/benches/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/src/benches/lexers_benchmark.rs` & `mountaineer-0.4.1.dev3/src/benches/lexers_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/src/benches/source_map_benchmark.rs` & `mountaineer-0.4.1.dev3/src/benches/source_map_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/src/benches/ssr_benchmark.rs` & `mountaineer-0.4.1.dev3/src/benches/ssr_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/src/lexers.rs` & `mountaineer-0.4.1.dev3/src/lexers.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/src/lib.rs` & `mountaineer-0.4.1.dev3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/src/logging.rs` & `mountaineer-0.4.1.dev3/src/logging.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/src/source_map.rs` & `mountaineer-0.4.1.dev3/src/source_map.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/src/ssr.rs` & `mountaineer-0.4.1.dev3/src/ssr.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/src/timeout.rs` & `mountaineer-0.4.1.dev3/src/timeout.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.1.dev2/Cargo.lock` & `mountaineer-0.4.1.dev3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mountaineer"
-version = "0.4.1-dev2"
+version = "0.4.1-dev3"
 dependencies = [
  "criterion",
  "deno_core_icudata",
  "env_logger",
  "lazy_static",
  "libc",
  "log",
```

### Comparing `mountaineer-0.4.1.dev2/pyproject.toml` & `mountaineer-0.4.1.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "mountaineer"
 dependencies = [ "pydantic", "fastapi", "inflection", "click", "uvicorn[standard]", "packaging", "watchdog", "pydantic-settings", "sqlmodel", "asyncpg", "sqlalchemy[asyncio]",]
 exclude = [ "fixtures", "ci_webapp", "create_mountaineer_app", "media", "docs_website", "benchmarking",]
 
 [tool.poetry]
 name = "mountaineer"
-version = "0.4.1.dev2"
+version = "0.4.1.dev3"
 description = ""
 authors = [ "Pierce Freeman <pierce@freeman.vc>",]
 readme = "README.md"
 
 [tool.mypy]
 warn_return_any = true
 warn_unused_configs = true
```

### Comparing `mountaineer-0.4.1.dev2/PKG-INFO` & `mountaineer-0.4.1.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mountaineer
-Version: 0.4.1.dev2
+Version: 0.4.1.dev3
 Requires-Dist: pydantic
 Requires-Dist: fastapi
 Requires-Dist: inflection
 Requires-Dist: click
 Requires-Dist: uvicorn[standard]
 Requires-Dist: packaging
 Requires-Dist: watchdog
```

