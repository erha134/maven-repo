# maven-repo
My maven Repo

### Usage

Add Repositories:
```gradle
repositories {
    // Add This
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
