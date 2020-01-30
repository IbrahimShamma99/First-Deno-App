deno run server.ts --allow-net --allow-env
curl -L https://getfly.fly.dev/install.sh | sh
flyctl auth login
flyctl apps create --builder deno
flyctl deploy
flyctl info