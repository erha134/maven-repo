中文 | [English](./readme.md)

# GaoShiLib

## 添加依赖

1. 添加仓库： [看这里](https://github.com/erha134/maven-repo/blob/main/README.md)

2. 添加依赖:

```gradle
dependencies {
    // 其他以来

    // ${minecraft_version} 是已经发布的 MC 版本（必须这个 mod 支持才行）
    // ${a/b} a, b二选一
    // ${gaoshilib_version} 是 mod 版本，可以在这里找到： https://github.com/MrCraftTeamMC/GaoShiLib/releases

    // 你可以把这些信息写进 'gradle.properties' 文件

    // For Fabric Loom / Quilt Loom / Architectury Loom
    modApi "cn.mrcraftteammc.gaoshilib:GaoShiLib-${fabric/xplat}-${minecraft_version}:${gaoshilib_version}" // 'xplat' 适用于任何 mod 加载器（插件不一定）, 'fabric' 适用于 architectury api (common项目) / fabric / quilt 

    // For Forge Gradle
    api fg.deobf("cn.mrcraftteammc.gaoshilib:GaoShiLib-forge-${minecraft_version}:${gaoshilib_version}")

    // For Others
    implementation "cn.mrcraftteammc.gaoshilib:GaoShiLib-${bukkit/bungeecord/sponge/velocity}-${minecraft_version}:${gaoshilib_version}"
}
```
