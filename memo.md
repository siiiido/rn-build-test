build

- yarn말고 npm 사용하는 것 추천
- npm install -g expo-cli ( expo-cli를 사용할 수 있게 해줌 )
- EAS Build는 무거운 작업임
- Android: build, sign까지 가능하지만 Google play developer에 upload는 못한다(맴버십 가입해야함 즉, 돈 내야함 -> one time $25)
- iOS: App store 역시 접근할려면 돈 내야함 $99

## 순서

1. npm install -g expo-cli
   - terminal에서 expo-cli 사용 할 수 있게 함
2. eas login
   - expo ID, PW로 로그인
3. eas build:configure
   - eas config 하기
   - Would you like to automatically create an EAS project for @tonyworld/my-expo-app? ... yes
   - Which platforms would you like to configure for EAS Build? » All
   - eas build --platform all = eas build --platform android + eas build --platform ios
