[中文](./readme_cn.md) | English

# GaoShiLib

## Add Dependencies

1. Add Repositories see [here](https://github.com/erha134/maven-repo/blob/main/README.md)

2. Add Deps:

```gradle
dependencies {
    // Other Dependencies

    // ${minecraft_version} can be any mc version in the folder
    // ${a/b} a or b choose one
    // ${gaoshilib_version} can be a version into the next folders or see https://github.com/MrCraftTeamMC/GaoShiLib/releases

    // You Also Can write them into 'gradle.properties'

    // For Fabric Loom / Quilt Loom / Architectury Loom
    modApi "cn.mrcraftteammc.gaoshilib:GaoShiLib-${fabric/xplat}-${minecraft_version}:${gaoshilib_version}" // 'xplat' is for any 'modloader', 'fabric' is for architectury api (common) / fabric / quilt 

    // For Forge Gradle
    api fg.deobf("cn.mrcraftteammc.gaoshilib:GaoShiLib-forge-${minecraft_version}:${gaoshilib_version}")

    // For Others
    implementation "cn.mrcraftteammc.gaoshilib:GaoShiLib-${bukkit/bungeecord/sponge/velocity}-${minecraft_version}:${gaoshilib_version}"
}
```
