## Collaborative Code Editor System Design.
![image](https://github.com/user-attachments/assets/95fb8a09-ae3d-4fe4-badc-0e85e72ef618)


## Code Compilation System Design.
![image](https://github.com/user-attachments/assets/830b079a-b63b-4762-b63c-eaff53f1950f)


## Video Demo 
[Watch on Youtube](https://youtu.be/afwZ4l_ZRMQ?si=WwQgzC0g1YT7C6Xk) - 
[Check LinkedIn Post](https://www.linkedin.com/feed/update/urn:li:activity:7263061074076205056)


## set up and run
```bash
cd ./app
```
write to all 4 services. 
```bash
cd ./frontend (eg. of 1 service)
npm i 
```
now open docker desktop.
after write in terminal

```bash
cd ../..
docker-compose up -d
```

then run 
```bash 
npm run dev
```

which start 4 different services.

## Demo 
![image](https://github.com/user-attachments/assets/30966c66-9984-4721-98cd-0b45709a1481)
![image](https://github.com/user-attachments/assets/78a842e2-0c12-4423-bbf9-fbacb41997fd)
![image](https://github.com/user-attachments/assets/ae41bc9f-fb0b-4044-9ea2-c809df57987b)

## Quick brush-up plan (Redis + Docker + Sockets)

If you want to get stronger with the main stack in this project, follow this short sequence:

1. **Docker fundamentals first**
   - Understand containers, images, volumes, networks, and `docker-compose`.
   - Practice: run `docker-compose up -d`, inspect running services, and check logs with `docker compose logs -f`.

2. **Redis basics and usage patterns**
   - Learn keys, TTL, pub/sub, caching, and queue-like workflows.
   - Practice: connect to Redis container and try `SET`, `GET`, `EXPIRE`, and pub/sub commands using `redis-cli`.

3. **Sockets and real-time communication**
   - Understand WebSocket lifecycle (`connect`, `message`, `disconnect`) and room/channel based messaging.
   - Practice: start the websocket service and trace how messages move between clients and backend services.

4. **Project-focused walkthrough**
   - Start the full stack with Docker.
   - Open the frontend, create a collaborative session, and watch logs from websocket + worker services.
   - Correlate: user action -> socket event -> Redis/pub-sub -> worker/server response.

This order (Docker -> Redis -> Sockets -> project internals) usually gives the fastest confidence boost.



