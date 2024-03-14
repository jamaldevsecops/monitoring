```
version: '3.3'

services:
  uptime-kuma:
    image: elestio/uptime-kuma:latest
    container_name: uptime-kuma
    restart: always
    environment:
      ADMIN_EMAIL: jamal.hossain@apsissolutions.com
      ADMIN_PASSWORD: "13F&b%"
    volumes:
      - uptime-kuma-data:/app/data
    ports:
      - '3001:3001'
    networks:
      - uptim-kuma

volumes:
  uptime-kuma-data:

networks:
  uptim-kuma:
    driver: bridge
```
