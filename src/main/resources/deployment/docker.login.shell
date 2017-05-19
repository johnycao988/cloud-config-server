#!/bin/sh

PID=$(docker inspect --format "{{ .State.Pid }}" $1)
echo "Getting docker container pid:"
echo $PID
echo "Starting to login docker container..."
nsenter --target $PID --mount --uts --ipc --net --pid
