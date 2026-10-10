# Orange

A lively light theme for Redmine (Redmine 7+) — a bold orange gradient
header, cream panels, and teal, pink, yellow and green accents. Surfaces are
kept muted (sand backgrounds, cream form fields) so the orange stays the
accent.

## Installation

1. Clone this theme ([https://github.com/zaburt/redmine_orange](https://github.com/zaburt/redmine_orange)) into the Redmine `themes/`
   directory at the application root (Redmine 7+) as `orange`:

   ```
   git clone https://github.com/zaburt/redmine_orange.git themes/orange
   ```

   The result should contain:

   ```
   themes/orange/stylesheets/application.css
   ```

   > Note: Redmine 6 and earlier used `public/themes/` instead of `themes/`.

2. Restart Redmine. In production, precompile assets:

   ```
   RAILS_ENV=production bin/rails assets:precompile
   ```

3. Go to `Administration -> Settings -> Display` and select "Orange" in the
   "Theme" drop-down list. Save your settings.

## Customize

1. Change `images/logo.svg` for the header logo (white text for the orange
   header), `images/logo-login.svg` for the full-color logo on the login
   page, and `favicon/favicon.svg` for the browser tab icon.
2. The palette is defined inline as hex values in
   `stylesheets/application.css`:

   | Role                  | Color     |
   |-----------------------|-----------|
   | Header gradient       | `#D9601A` → `#E9A63E` |
   | Page background       | `#EBDCC8` |
   | Content background    | `#F6EEE2` |
   | Panels                | `#FBF6EE` |
   | Text                  | `#4A2A12` |
   | Links / buttons       | `#D84A00` / `#E04E00` |
   | Teal accent           | `#2C8C93` |
   | Pink accent           | `#D9577F` |
   | Success               | `#3E9B63` |
   | Error                 | `#D32F2F` |

3. In production, re-run `assets:precompile` after editing any theme file.

## License

Licensed under [GNU GPLv2](LICENSE).

Copyright (c) 2026 Onur Küçük (onur [at] delipenguen.net)
