FROM debian:bookworm-slim
RUN apt-get update && apt-get install -y --no-install-recommends g++ && rm -rf /var/lib/apt/lists/*
WORKDIR /app
COPY main.cpp .
RUN g++ -std=c++17 -O2 -pthread main.cpp -o hospital
EXPOSE 3000
CMD ["./hospital"]
