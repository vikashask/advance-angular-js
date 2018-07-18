## Deploying your Angular application to a remote server.

## 1.Start with the development build
    ng build

## 2.Copy everything within the output folder (dist/ by default) to a folder on the server.

## 3.If you copy the files into a server sub-folder, append the build flag, --base-href and set the <base href> appropriately.
    For example, if the index.html is on the server at /app/index.html, set the base href to <base href="/app/"> like this.
    ng build --base-href=/app/

