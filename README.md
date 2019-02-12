# Технології створення програмних продуктів для мобільних платформ

### Опис курсу

Курс складається з теоретичних занять та практичних занять.

Завданням для практичних занять курсу є створення концепції та розробка мобільного ПЗ для будь-якої сучасної мобільної платформи нативними або альтернативними засобами. Завдання має бути зробленим командою не більше 3 студентів. У розробленому продукті бажана наявність наступних пунктів:

* Робота із мережею
* Робота із БД або файлами в internal/external storage застосунку
* Відповідність HIG для iOS-застосунків та Material Design для Android-застосунків
* Робота з сервісами телефону (камера, сервіси локації)
* Робота з зовнішнім API (можна власним), використання SDK
* Використання кастомних анімацій

#### Дедлайни і вимоги

Розробку проекту має бути завершено до середини травня. У фінальному проекті не всі етапи мають бути обов'язково присутні. Обов'язковими для всіх проектів є етапи роботи 1-3. Оцінка залежить від якості реалізації (архітектурні рішення) і наявності в фінальному проекті відтворення хоча б декількох запропонованих рекомендованих етапів. 
* Для першої атестації необхідно виконати роботу 1.
* Для другої атестації необхідно виконати роботи 1-3.

### Обов'язкові етапи роботи:

1. Створення концепції продукту (ЛР №1)

  * Розподілитись на команди (до 3 людей в залежності від складності задачі)
  * Cтворити ідею продукту, описати її.
  * Cтворити репозиторій в GitHub для подальшої роботи над проектом. Файл readme має містити:
  
    * Короткий опис ідеї
    * Визначення технічних вимог до застосунку (версія платформи, permissions)
    * Короткий опис потенційної аудиторії
    
  * Створити папку docs та додати туди наступні файли:
  
    * Use-Case діаграма (з мінімальним ступенем деталізації, суто для пояснення функціоналу застосунку)
    * Raw-прототип (за бажанням)

  Написати про склад команди розробників та надати посилання на репозиторій проекту [сюди](https://github.com/kpimobiledev/MobileDev/issues/3) (без дублювання)

2. Створення дизайн-прототипу застосунку (ЛР №2)

  * Ознайомитись із загальними концепціями дизайну для iOS та Android
  * Розробити дизайн для застосунку, концепцію якого було **затверджено** у результаті виконання ЛР №1

  Рекомендоване ПЗ для створення/роботи із дизайном:
  * [InVision](https://www.invisionapp.com)
  * [NinjaMock](https://ninjamock.com)
  * [Sketch](https://www.sketchapp.com)

  Матеріали для ознайомлення:

  * Android
    * [Material Design for Android](https://developer.android.com/design/material/index.html)
    * [Material Design Guidelines](https://material.io/guidelines/)
    * [Material Design Principles (Udacity course)](https://www.udacity.com/course/material-design-for-android-developers--ud862)
    * [UX for mobile developers (Udacity course)](https://www.udacity.com/course/ux-design-for-mobile-developers--ud849)
    * [MaterialUp: the best examples of material design](https://material.uplabs.com)
  * iOS
    * [iOS Human Interface Guidelines](https://developer.apple.com/ios/human-interface-guidelines/overview/design-principles/)
    * [iOSUp: the best examples of iOS design](https://ios.uplabs.com)
  * Sketch
    * [Розробка дизайну у Sketch](https://www.youtube.com/watch?v=mlgI4u_X8sU)

  Термін виконання: до 21.03

3. Перенесення дизайну у застосунок. Створення прототипу .

Завданням ЛР є імплементація дизайн-прототипу засобами SDK, яке ви використовуєте в залежності від платформи.. Загальною вимогою до розміток є відповідність дизайну та внесеним до нього рекомендаціям, стійкість до змін конфігурації телефону. Необхідно ознайомитися із документацією і ретельно продумати, які операції можна виокремити у вашому застосунку, яку архітектуру краще побудувати для реалізації необхідного функціоналу. У результаті ЛР має бути створено застосунок, який містить всі необхідні переходи між екранами, без реалізації сервісів безпоередньо.
  
   Матеріали для ознайомлення:
   * [Android Basics Tutorial](https://developer.android.com/guide/)
   * [Android Jetpack](https://developer.android.com/jetpack/)
   * [Android Basics: User Interface (Udacity course)](https://www.udacity.com/course/android-development-for-beginners--ud837)
   * [Android Basics: Multi-screen applications (Udacity course)](https://www.udacity.com/course/android-basics-multi-screen-apps--ud839)

### Рекомендовані етапи роботи:

4. Реалізація взаємодії із мережею.

Завданням ЛР є розробка частини застосунку, відповідну за взаємодію із мережею. Завдання ЛР включає:
    * Робота із сторонніми API або SDK, необхідних для застосунку (наприклад, API/SDK соціальних мереж, засобів оплати, SDK Google Maps тощо)
    * Робота із засобами аналітики застосунку або реклами (Firebase Analytics, AdMob)

   Матеріали для ознайомлення:
   * [Performing network operations](https://developer.android.com/training/basics/network-ops/index.html)
   * [Android Basics: Networking (Udacity course)](https://www.udacity.com/course/android-basics-networking--ud843)
   Додаткову інформацію щодо конкретних API/SDK можна знайти на сайтах провайдерів API/SDK.

5. Робота із особливостями пристрою

Завданням ЛР є розробка частини застосунку, відповідної за роботу із особливостями пристрою. Завдання ЛР включає роботу із:
    * Камерою
    * GPS
    * Bluetooth
    * Мікрофон
    * Fingerprint
    * NFC [тощо](https://developer.android.com/guide/topics/manifest/uses-feature-element.html)

6. Збереження даних.

  Завданням ЛР є розробка частини застосунку, відповідної за роботу із збереженням даних (БД, файлова система тощо). Можна використовувати будь-який доцільний засіб збереження даних, якщо необхідно.

   Матеріали для ознайомлення:
   * [Saving data in Android](https://developer.android.com/training/basics/data-storage/index.html)
   * [Android Basics: Data Storage (Udacity course)](https://www.udacity.com/course/android-basics-data-storage--ud845)

Термін здачі лабораторних робіт №3-8 — термін здачі курсової роботи студентів АСОІУ. Саме за тим, який функціонал та особливості має ваш застосунок, наскільки його добре відлагоджено, буде висталено оцінку за курсову роботу та зараховано відповідні лабораторні роботи.

## Матеріали курсу

Слайди лекцій буде викладено в поточному репозиторії.
До вивчення рекомендовано наступні ресурси:

### Android

* [Android Developers: Tutorials and Reference](https://developer.android.com/index.html)
* [Android Udacity courses list](https://www.udacity.com/courses/android)

#### Intermediate
* [Material Design Principles](https://www.udacity.com/course/material-design-for-android-developers--ud862)
* [Developing Android Apps (strongly recommended)](https://www.udacity.com/course/new-android-fundamentals--ud851)

#### Advanced
* [Android Performance](https://www.udacity.com/course/android-performance--ud825)
* [Advanced Android App Development](https://www.udacity.com/course/advanced-android-app-development--ud855)

### iOS

#### Beginner
* [Swift Syntax](https://www.udacity.com/course/learn-swift-programming-syntax--ud902)
* [Objective-C Syntax](https://www.udacity.com/course/objective-c-for-swift-developers--ud1009)

#### Intermediate
* [AutoLayout](https://www.udacity.com/course/auto-layout--ud1026)
* [Networking](https://www.udacity.com/course/ios-networking-with-swift--ud421)
* [UIKit Fundamentals](https://www.udacity.com/course/uikit-fundamentals--ud788)

#### Advanced
* [GCD](https://www.udacity.com/course/grand-central-dispatch-gcd--ud576)
* [Xcode debugging](https://www.udacity.com/course/xcode-debugging--ud774)
* [Persistent storage and Core Data](https://www.udacity.com/course/ios-persistence-and-core-data--ud325)

## Зворотній зв'язок

* [Artem Chernenkiy](https://telegram.me/gy_fk) in Telegram
* [Lidiya Ivanova](https://telegram.me/lidaamber) in Telegram
