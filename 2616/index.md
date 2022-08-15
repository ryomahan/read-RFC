## 导言

### 术语

connection

message

request

response

resource

entity

representation

content negotiation

variant

client

user agent

server

origin server

proxy

gateway

tunnel

cache

cacheable

first-hand

explicit expiration time

heuristic expiration time

agent

freshness lifetime

fresh

stale

semantically transparent

validator


upstream/downstream
用来描述消息流，所有的消息都是从上游流向下游

inbound/outbound


### Overall Operation | 大致流程

HTTP 协议是一个 请求/响应 协议。

客户端以 request method, URI and protocol version 的形式向服务器发送请求。然后通过与服务器与服务器的 connection 传递一条类似 [MIME][1] 的消息，其中包括：request modifiers, client information and possible body content。

服务器通过一个状态行进行响应，其中包括：the message's protocol version and a success or error code，然后和请求一样通过 connection 传递一条类似 MIME 的消息，其中包括：server information, entity metainformation and possible entity-body content。



[1]: https://en.wikipedia.org/wiki/MIME
