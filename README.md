# Figura File Sync

一个Fabric模组，让Figura可以同步任意文件（不只是avatar模型）给多人模式的其他玩家。

## 功能

- 支持同步任意文件类型（FBX、OBJ、GLTF、PNG、JSON、LUA等）
- 保持文件相对路径结构
- 通过Figura后端同步给其他玩家

## 依赖

- Minecraft 1.20.1
- Fabric Loader 0.14.25+
- Figura mod

## 安装

1. 安装 [Figura](https://modrinth.com/mod/figura) 模组
2. 下载本模组的 `jar` 文件
3. 放入 `.minecraft/mods` 文件夹

## 使用方法

```
/figurasync upload <文件路径>   - 上传文件同步给其他玩家
/figurasync list                - 列出已同步文件
/figurasync reload              - 重新加载配置
/figurasync help                - 显示帮助
```

### 示例

```
/figurasync upload mods/mytexture.png
/figurasync upload resourcepacks/mypack/assets/logo.png
/figurasync upload config/myconfig.json
```

## 支持的文件格式

- 3D模型: fbx, obj, gltf, glb
- 纹理: png, jpg, jpeg, gif, bmp
- 数据: json, nbt
- 脚本: lua, luac
- 音频: wav, ogg, mp3

## 构建

```bash
./gradlew build
```

输出: `build/libs/figura-file-sync-1.0.0-fabric-mc1.20.1.jar`

## 许可证

MIT License
