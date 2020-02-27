# netty-http2-server-demo
http2-server-demo

## usage

// params customed by env of linux

// System.getenv("GLAHA_HTTP2_PORT");

// System.getenv("GLAHA_HTTP2_SSL"); true or null

// System.getenv("GLAHA_HTTP2_RESPONSE_SIZE"); big or small

// -Dssl=true or null

java -Xbootclasspath/p:/alpn-boot-8.1.13.v20181017.jar -jar netty-http2-server-x.y-SNAPSHOT.jar

## test commands

### http

curl -i  http://127.0.0.1:8080

### http2 h2c

curl -i --http2   http://127.0.0.1:8080

### http2 clear text priorknowledge

curl -i --http2-pri http://127.0.0.1:8080

### http2 h2

curl -i -k --http2 https://127.0.0.1:8443