# {Service Name} 🔥

# {Description}

#### Feature
- [x]  Feature 1
- [x]  Feature 2
- [x]  Feature 3
- [x]  Feature 4


#### System requirements Development
- [x]  docker
- [x]  Jaeger
- [x]  MongoDb

#### Prototype
<p align="left">
    <a href="https://github.com/touchtechnologies-product/go-blueprint-clean-architecture">Touch Go Blueprint</a>
</p>

### Api Specification

URL: <a href="http://example.swagger-api-touch.com">example.swagger-api-touch.com</a>

### Pre-Require

Mockery
```
GO111MODULE=off go get github.com/vektra/mockery/.../
```

### Installation

```
  git clone https://git.touchdevops.com/touchtechnologies/payment-gateway.git
  cd gogo-blueprint
  go mod download
```



### Testing 
unit testing command

```
  go test ./... -v
```

integrating testing command

```
  go test ./... -tags integration
```


### Generate Mocks

generate mocks from interfaces for unit testing

```
  go generate ./...
```


### Local development
development in local start mongodb jaeger

```
cd development
source ./local.env
docker-compose up -d
```

### Tracing with Jaeger
please see in the example code implement jaeger wrap service ```service/company/withtracer```


### Others

- Uber golang style guide [link](https://github.com/uber-go/guide)
- Practical Go: Real world advice for writing maintainable Go programs [link](https://dave.cheney.net/practical-go/presentations/qcon-china.html?fbclid=IwAR2_D2Y2HXVYUNiG3LctB0kF64YKzGUatcIHm_sLYwm9SEqEKWAd76G7NAU)
