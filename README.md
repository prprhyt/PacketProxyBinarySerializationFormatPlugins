# BinarySerializationFormatPlugins(CBOR, MessagePack) for PacketProxy

This repository provides binary serialization format plugins for [PacketProxy](https://github.com/DeNA/PacketProxy).

This repository include following plugins,

- CBOR2JSON: CBOR <-> JSON plugin
- MessagePack2JSON: MessagePack <-> JSON plugin.

## Build & Install

```bash
$ git clone git@github.com:prprhyt/PacketProxyBinarySerializationFormatPlugins.git
$ cd PacketProxyBinarySerializationFormatPlugins/
$ ./gradlew shadowJar
$ cp build/libs/PacketProxyPlugin-1.0.0-all.jar ~/.packetproxy/plugins/BinarySerializationFormatPlugins.jar
```

After finishing the installation, you can select `CBOR2JSON` and `MessagePack2JSON` encode module in servers panel.

# Licences

Apache License 2.0
