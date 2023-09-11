中文 | [English](./README.md)

# maven-repo
我的 Maven 仓库

## Usage

添加仓库:
```gradle
repositories {
    // 添加这个
    maven {
        name = "MrCraftTeamMC Release Maven"
        url = "https://raw.githubusercontent.com/erha134/maven-repo/main/releases/"
    }
    maven {
        name = "MrCraftTeamMC Snapshot Maven"
        url = "https://raw.githubusercontent.com/erha134/maven-repo/main/snapshot/"
    }
}
```
