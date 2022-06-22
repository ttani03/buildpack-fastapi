load("ext://pack", "pack")

docker_compose('docker-compose.yml')
pack(
    'buildpack-fastapi',
    builder='paketobuildpacks/builder:base',
    live_update=[
        sync('./', '/workspace'),
    ]
)
