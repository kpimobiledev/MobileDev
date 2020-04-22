# Технології створення програмних продуктів для мобільних платформ

### Опис курсу

Курс складається з 18 лекцій, 9 лабораторних робіт і курсового проекту, 2 МКР.
Пропорції оцінювання:

##### Дисципліна
* МКР-1: 10 балів, обов'язково для першої атестації
* МКР-2: 10 балів, обов'язково для другої атестації
* Лабораторні роботи: 80 балів

##### Курсова – 100 балів відповідно реалізованому проекту

Завданням для лабораторних занять курсу і курсового проекту є створення концепції та розробка мобільного ПЗ для будь-якої сучасної мобільної платформи нативними або гібридними засобами. Завдання має бути зробленим командою не більше 3 студентів. У розробленому продукті бажана наявність наступних пунктів:

* Робота із мережею
* Робота із БД або файлами в internal/external storage застосунку
* Відповідність HIG для iOS-застосунків та Material Design для Android-застосунків
* Робота з сервісами телефону (камера, сервіси локації тощо)
* Робота з зовнішнім API (можна власним), використання SDK
* Використання кастомних анімацій

#### Лабораторні роботи і курсовий проект
Курсовий проект і лабораторні роботи можна поєднати в у виконанні. Курсовий проект складається з етапів, кожен з яких є лабораторною роботою. 
* Вибір ідеї, вибір інструментарію
* Створення інтерактивного прототипу застосунку
* Архітектура застосунку
* Імплементація UI застосунку
* Імплементація бізнес-логіки користувача
* Імплементація взаємодії з мережею
* Імплементація зберігання даних локально
* Імплементація взаємодії з hardware пристрою
* Імплементація тестів

Ви можете виконувати лабораторні роботи поетапно або захистити їх всі разом як цілісний проект. Ви можете зробити це протягом семестру на практичних заняттях або наприкінці семестру. 
##### Обов'язкові компоненти проекту (оцінка E-D)
* Вибір ідеї, вибір інструментарію – більш детально у відкритому issue
* Створення інтерактивного прототипу застосунку
* Архітектура застосунку
* Імплементація UI застосунку
* Імплементація бізнес-логіки користувача

##### Додаткові компоненти проекту, хоча б 1, більше – краще (оцінка C-А) 
* Імплементація взаємодії з мережею
* Імплементація зберігання даних локально
* Імплементація взаємодії з hardware пристрою

##### Для перфекціоністів (А100)
* Імплементація тестів

Курсовий проект також має включати текстовий опис поетапного виконання роботи, обсяг пояснювальної записки ~ 20 сторінок.

#### Дедлайни і вимоги

1. Лабораторні роботи / курсовий проект – середина травня
2. МКР-1 – проводиться орієнтовно на лекції 8
3. МКР-2 – проводиться орієнтовно на лекцїї 15

### Детальніше про етапи курсового проекту / лабораторні

##### 1. Вибір ідеї, вибір інструментарію

* Розподілитись на команди (до 3 людей в залежності від складності задачі)
* Cтворити ідею продукту, описати її.
* Cтворити репозиторій в GitHub для подальшої роботи над проектом. Файл readme має містити:
    * Короткий опис ідеї
    * Визначення технічних вимог до застосунку (версія платформи, permissions)
    * Короткий опис потенційної аудиторії

Написати про склад команди розробників та надати посилання на репозиторій проекту [сюди](https://github.com/kpimobiledev/MobileDev/issues/4) (без дублювання)

##### 2. Створення дизайн-прототипу застосунку

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

##### 3. Архітектура застосунку

Завданням ЛР є розробка архітектури програмного забезпечення. Потрібно обрати архітектурний підхід до розробки вашого застосунку серед відомих підходів MVC, MVP, MVVM, VIPER або розробити власну архітектуру, обрґрунтувати її доцільність для вашого проекту. Для демонстрації архітектури розробити схему взаємодії шарів застосунку і опублікувати цю схему в репозиторії.

##### 4. Перенесення дизайну у застосунок. Створення прототипу.

Завданням ЛР є імплементація дизайн-прототипу засобами SDK, яке ви використовуєте в залежності від платформи. Загальною вимогою до розміток є відповідність дизайну та внесеним до нього рекомендаціям, стійкість до змін конфігурації телефону. Необхідно ознайомитися із документацією і ретельно продумати, які операції можна виокремити у вашому застосунку, яку архітектуру краще побудувати для реалізації необхідного функціоналу. У результаті ЛР має бути створено застосунок, який містить всі необхідні переходи між екранами, без реалізації сервісів безпоередньо.
  
Матеріали для ознайомлення:
* [Android Basics Tutorial](https://developer.android.com/guide/)
* [Android Jetpack](https://developer.android.com/jetpack/)
* [Android Basics: User Interface (Udacity course)](https://www.udacity.com/course/android-development-for-beginners--ud837)
* [Android Basics: Multi-screen applications (Udacity course)](https://www.udacity.com/course/android-basics-multi-screen-apps--ud839)

##### 5. Реалізація бізнес-логіки.

Завданням ЛР є розробка бізнес-логіки застосунку: обробка подій користувача, навігація, логіка застосунку окрім взаємодії з мережею і збереження даних локально.

##### 6. Реалізація взаємодії із мережею.

Завданням ЛР є розробка частини застосунку, відповідну за взаємодію із мережею. Завдання ЛР включає:
* Робота із сторонніми API або SDK, необхідних для застосунку (наприклад, API/SDK соціальних мереж, засобів оплати, SDK Google Maps тощо)
* Робота із засобами аналітики застосунку або реклами (Firebase Analytics, AdMob)

Матеріали для ознайомлення:
* [Performing network operations](https://developer.android.com/training/basics/network-ops/index.html)
* [Android Basics: Networking (Udacity course)](https://www.udacity.com/course/android-basics-networking--ud843)

Додаткову інформацію щодо конкретних API/SDK можна знайти на сайтах провайдерів API/SDK.

##### 7. Робота із особливостями пристрою

Завданням ЛР є розробка частини застосунку, відповідної за роботу із особливостями пристрою. Завдання ЛР включає роботу із:
* Камерою
* GPS
* Bluetooth
* Мікрофон
* Fingerprint
* NFC [тощо](https://developer.android.com/guide/topics/manifest/uses-feature-element.html)

##### 8. Збереження даних.

Завданням ЛР є розробка частини застосунку, відповідної за роботу із збереженням даних (БД, файлова система тощо). Можна використовувати будь-який доцільний засіб збереження даних, якщо необхідно.

Матеріали для ознайомлення:
* [Saving data in Android](https://developer.android.com/training/basics/data-storage/index.html)
* [Android Basics: Data Storage (Udacity course)](https://www.udacity.com/course/android-basics-data-storage--ud845)

##### 9. Розробка тестів для застосунку

Завданням є написання Unit-тестів для бізнес-логіки застосунку і написання UI-тестів для двох головних екранів вашого застосунку на ваш вибір.

## Матеріали курсу

Лекції:
* [Лекція 1](https://docs.google.com/presentation/d/1Bt68iRD6yCuw_OZpZWIMYw7wazEzxSpkWIa-ugUlUhg/edit?usp=sharing)
* [Лекція 2-3](https://docs.google.com/presentation/d/1gcOsJ-qYn4JEXr5_2tdbOv3GhcIL-KfJM59cAUtVi8w/edit?usp=sharing)
* [Лекція 4](https://docs.google.com/presentation/d/1bvOismyq51QEyryyV7TMYvAeVtsq48tQO7T5fZgzDjE/edit?usp=sharing)
* [Лекція 5](https://docs.google.com/presentation/d/19N5PKXLtMx_FfPzHBcadmXNRq5RL8DDP_PMGMYr-i_o/edit?usp=sharing)
* [Лекція 6](https://docs.google.com/presentation/d/1h27pW4FqvHXq5aQYJoWQjTcrIbm0duzX3AzaYb4ZQc0/edit?usp=sharing)
* [Лекція 7](https://docs.google.com/presentation/d/1CducSVcCpO7Ie9cgJEG6Rk6VnntcO-z3VqfIy4y_glE/edit?usp=sharing)
* Лекція 8 (МКР-1)
* [Лекція 9](https://docs.google.com/presentation/d/1zf0xMMNBWoVAs19VpCrD75dqlR_J6zLJlh5FijfiICQ/edit?usp=sharing)
* [Лекція 10](https://docs.google.com/presentation/d/1vbMkXhSCMD7qFI3O9wSpepnwXv2bP4GpHt9qIKXzYAA/edit?usp=sharing)
* [Лекція 11](https://docs.google.com/presentation/d/1rR-km104dmU2oZmvPCSuvIKmgAovOKqZj2KnmFCUc_s/edit?usp=sharing)
* [Лекція 12](https://docs.google.com/presentation/d/1BqnbDejek_5WB4UPSwgH19VR-Ctdj5kPnCx9rFC72pE/edit?usp=sharing)

До вивчення рекомендовано наступні ресурси:

### Android

* [Android Developers: Tutorials and Reference](https://developer.android.com/index.html)
* [Android Udacity courses list](https://www.udacity.com/courses/android)
* [Kotlin language reference](https://kotlinlang.org )
* [Android codelabs (from Google)](https://codelabs.developers.google.com/?cat=Android)

#### Intermediate
* [Material Design Principles](https://www.udacity.com/course/material-design-for-android-developers--ud862)
* [Developing Android Apps (for Java developers)](https://www.udacity.com/course/new-android-fundamentals--ud851)
* [Developing Android Apps (for Kotlin developers)](https://www.udacity.com/course/developing-android-apps-with-kotlin--ud9012)

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
