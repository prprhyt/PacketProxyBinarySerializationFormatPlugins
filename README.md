# BinarySerializationFormatPlugins(CBOR, MessagePack) for PacketProxy

This repository provides binary serialization format plugins for [PacketProxy](https://github.com/DeNA/PacketProxy).

This repository include following plugins,

- CBOR2JSON: CBOR <-> JSON plugin
- MessagePack2JSON: MessagePack <-> JSON plugin.

This plugin was created based on [this template(DeNA/PacketProxyPlugin)](https://github.com/DeNA/PacketProxyPlugin).

## Install

### Install from released JAR file

1. Go to release page.
https://github.com/prprhyt/PacketProxyBinarySerializationFormatPlugins/releases
1. Download latest version jar file.
1. Execute `open ~/.packetproxy/plugins` in Terminal. (If it does not exist, you should create it.)
1. Drug jar file to `~/.packetproxy/plugins` and drop it.
1. Run PacketProxy, you can select `CBOR2JSON` and `MessagePack2JSON` encode module in servers panel.

### Build & Install from source code yourself.

```bash
$ git clone git@github.com:prprhyt/PacketProxyBinarySerializationFormatPlugins.git
$ cd PacketProxyBinarySerializationFormatPlugins/
$ ./gradlew shadowJar
$ cp build/libs/PacketProxyPlugin-1.0.0-all.jar ~/.packetproxy/plugins/BinarySerializationFormatPlugins.jar
```

After finishing the installation, you can select `CBOR2JSON` and `MessagePack2JSON` encode module in servers panel.

## ScreenShot

CBOR2JSON
![CBOR2JSON](https://github.com/prprhyt/PacketProxyBinarySerializationFormatPlugins/raw/master/screenshot/cbor2json.png)

MessagePack2JSON
![MessagePack2JSON](https://github.com/prprhyt/PacketProxyBinarySerializationFormatPlugins/raw/master/screenshot/msgpack2json.png)

# Licences

Apache License 2.0
