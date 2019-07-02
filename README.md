
# Docker for API

You can build and run the docker using the following process:

Cloning
```console
gti clone https://github.com/jqueguiner/uncolorization.git uncolorization
```

Building Docker
```console
cd uncolorization && docker build -t uncolorization -f Dockerfile .
```

Running Docker
```console
echo "http://$(curl ifconfig.io):5000" && docker run -p 5000:5000 -d uncolorization
```

Calling the API for programming language detection
```console
curl -X POST "http://MY_SUPER_API_IP:5000/process" -H "accept: application/json" -H "Content-Type: application/json" -d '{"url":"https://i.ibb.co/x3srpR0/input.jpg"}'
```
