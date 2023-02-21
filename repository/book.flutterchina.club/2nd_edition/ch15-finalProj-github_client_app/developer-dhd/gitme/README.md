### [15.1 Github客户端示例 | 《Flutter实战·第二版》](https://book.flutterchina.club/chapter15/intro.html)

<br/>

作者未提供 source project，且展示的 code snippet 開發時間已經是幾年前，代碼有部分已過時，不再適用。

e.g. GitHub API 目前已不支援帳號密碼登陸，需使用 [创建个人访问令牌 - GitHub Docs](https://docs.github.com/zh/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) 。

<br/>
↪ &nbsp;搜尋到的其他開發者的實作 [developer-dhd/gitme: github client, github flutter learn, flutter学习，flutter练手项目](https://github.com/developer-dhd/gitme)


</br>

#### Ref :
- GitHub API : &nbsp;[Users - GitHub Docs](https://docs.github.com/en/rest/users/users?apiVersion=2022-11-28)


<br/>

----

<br/>

Run debugger via [IntelliJ IDEA](https://download.jetbrains.com/idea/ideaIC-2022.3.exe?_gl=1*1hnijhq*_ga*MTI4MTM3NjM4NC4xNjUwNTUwMTg1*_ga_9J976DJZ68*MTY3ODA5MjQyOC4xOC4xLjE2NzgwOTI0NjYuMC4wLjA.&_ga=2.115582086.1629192515.1678092429-1281376384.1650550185)

1. Follow [Flutter打包Android应用apk签名 | DecoderX](https://decoderx.cc/posts/59b1662f.html) to generate file `key.jks`, then put it to the location `developer-dhd\gitme\key.jks` .

2. apply [self adaptive patch](./0001-self-modification-for-run-demo-via-IntelliJ-IDEA-deb.patch)

3. Okay, thus it's able to run debugger via [IntelliJ IDEA](https://download.jetbrains.com/idea/ideaIC-2022.3.exe?_gl=1*1hnijhq*_ga*MTI4MTM3NjM4NC4xNjUwNTUwMTg1*_ga_9J976DJZ68*MTY3ODA5MjQyOC4xOC4xLjE2NzgwOTI0NjYuMC4wLjA.&_ga=2.115582086.1629192515.1678092429-1281376384.1650550185)

    a). Open project in IDEA

    b). After a while, IDEA will pop up a UI prompting you to execute `flutter pub get`.

    c). Launch the Android emulator.

    d). Select fullter device to `Android Emulator`, and it's okay to run debbugger (Shift + F9) now.

    e). When app launched in Android emulator, type your GitHub account and the [__Personal access tokens (classic)__](https://github.com/settings/tokens), NOT the password !

