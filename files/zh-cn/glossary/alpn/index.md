---
title: 应用层协议协商
slug: Glossary/ALPN
tags:
  - ALPN
  - TLS
translation_of: Glossary/ALPN
---
**应用层协议协商**（**Application-Layer Protocol Negotiation**，简称**ALPN**）是 {{Glossary("TLS")}} 的一个扩展，故而应用层协议在协商加密协议的过程中，避免了额外的往返通讯开销。

| 协议                                           | 标识符字节序列                                         |
| ---------------------------------------------- | ------------------------------------------------------ |
| {{Glossary("HTTP")}}/1.1               | `0x68 0x74 0x74 0x70 0x2F 0x31 0x2E 0x31` ("http/1.1") |
| {{Glossary("HTTP 2", "HTTP/2")}}   | `0x68 0x32` ("h2")                                     |
| HTTP/2 over cleartext {{Glossary("TCP")}} | `0x68 0x32 0x63` ("h2c")                               |

## Specifications

| Specification    | Status   | Notes      |
| ---------------- | -------- | ---------- |
| {{RFC(7301)}} | IETF RFC | 初始化定义 |

## See also

- [IANA registered ALPN identifiers](https://www.iana.org/assignments/tls-extensiontype-values/tls-extensiontype-values.xhtml#alpn-protocol-ids)
