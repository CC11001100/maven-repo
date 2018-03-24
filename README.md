## 个人Maven仓库

### 用途
用于发布个人项目方便集成到其它项目中。

---
### 使用方式
首先添加仓库：
```
<repositories>
    <repository>
        <id>maven-repo-cc11001100</id>
        <url>https://raw.github.com/cc11001100/maven-repo/[分支名字]/</url>
        <snapshots>
            <enabled>true</enabled>
            <updatePolicy>always</updatePolicy>
        </snapshots>
    </repository>
</repositories>
```
然后添加dependency：
```
<dependency>
    <groupId>cc11001100</groupId>
    <artifactId>项目名字</artifactId>
    <version>版本号</version>
</dependency>
```
即可将依赖集成进来。

