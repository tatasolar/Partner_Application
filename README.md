# Frontend deployment

This app is a static HTML page; there is no npm build step. The production files
are `index.html` and `tata-power-logo.svg`.

## GitHub Pages

Upload the contents of this folder to the publishing root (or publish the
folder from a branch/workflow). Ensure both files are in the same directory.
The page calls the API must have a valid
TLS certificate and allow this site's origin in `CORS_ORIGINS`.

For a different backend domain, change the non-local `API_BASE_URL` in
`index.html` before publishing. Do not put database credentials or the admin
PIN in frontend files; all files served to a browser are public.
