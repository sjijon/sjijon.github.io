Start this Jekyll site locally and open it in a new Safari window.

## Steps

1. From the project root, check whether Jekyll is already serving on port 4000 (e.g. look for an existing `jekyll serve` process or that `http://localhost:4000` responds).
2. If it is not running, start the server in the background from the project root:
   ```bash
   jekyll serve
   ```
   If the project uses Bundler (`Gemfile` present), use:
   ```bash
   bundle exec jekyll serve
   ```
   Wait until the server is ready (look for the “Server address” / localhost:4000 message).
3. Open a **new Safari window** pointed at the local site:
   ```bash
   osascript -e 'tell application "Safari" to activate' -e 'tell application "Safari" to make new document with properties {URL:"http://localhost:4000"}'
   ```
4. Tell the user the site is available at http://localhost:4000 and that Safari was opened.

Do not stop an already-running Jekyll server; reuse it. Do not run tests.
