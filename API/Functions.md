* **[Functions](#functions)**
* **[Hooks](#hooks)**
* **[Structs](#structs)**
* **[Examples](#Examples)**

## Functions
* **[Log(string)](#Log)**
* **[Sleep(int ms)](#Sleep)**
* **[format(pattern, ...)](#format)**
* **[SendPacket(int type, string packet)](#SendPacket)**
* **[SendPacketRaw(GamePacket)](#SendPacketRaw)**

## Hooks

## Structs
    std::string keys[18] = { "type", "objtype", "count1", "count2", "netid", "itemid", "flags", "float1", "int_data", "pos_x", "pos_y", "pos2_x", "pos2_y", "float2", "tile_x", "tile_y", "data_size", "data" };

### GamePacket
| Description | Name | Type |
|:------------|:----:|:-----|
| Packet Type |  **type** | Number |
| Object Type |  **objtype** | Number |
| None |  **count1** | Number |
| None |  **count2** | Number |
| Packet NetID |  **netid** | Number |
| Packet Flags |  **flags** | Number |
| Packet Type |  **float1** | Number |
| Packet Type |  **float2** | Number |
| Packet posx |  **pos_x** | Number |
| Packet posy |  **pos_y** | Number |
| Packet pos2x |  **pos2_x** | Number |
| Packet pos2y |  **pos2_y** | Number |
| Packet tilex |  **tile_x** | Number |
| Packet tiley |  **tile_y** | Number |
| Packet datasize |  **data_size** | Number |
| Packet intdata |  **data** | Number |

## Examples

### Log
```lua
-- logs to growtopia console
Log("Hello World!")
```

### Sleep
```lua
-- sleeps, waits
Sleep(500) -- sleeps 500 ms
```

### format
```lua
-- formats string
test = "uhmm yeah":format("well its -> {}")
Log(test)
```

### SendPacket
```lua
-- Sends Packet to game
SendPacket(2, "action|input\n|text|Hello from Apollo Executor")
```

### SendPacketRaw
```lua
-- Sends Raw Packet to game
packet = GamePacket()
packet.type = 0
packet.flags = 48
SendPacketRaw(packet) -- Character's face returns to left
```
