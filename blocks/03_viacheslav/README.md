# Частина 3: Керування і прийняття рішень

Існує три види роботизованих програм: дистанційне керування, штучний інтелект і гібрид. [3.1.][3.1.]

## Зворотний зв'язок

**Зворо́тний зв'язо́к**  — вплив результату функціонування будь-якої системи
на характер її подальшого функціонування. [3.1.1.][3.1.1.]

За характером впливу зворотній зв'язок поділяють на *позитивний* і *негативний* (balancing feedback).

*Позитивний зворотний зв'язок* впливає на систему таким чином, що збільшує вихідний результат її функціонування.
...завдяки цьому в системі виникають незатухаючі коливання.

*Негативний зворотний зв'язок* впливає на систему таким чином, що зменшує вихідний результат її функціонування.
...при цьому також підвищується стійкість системи та зменшується похибка та інерційність системи.

Whereas positive feedback tends to instability via exponential growth,
oscillation or chaotic behavior, negative feedback generally promotes stability. [3.1.2.][3.1.2.]

> Виникає цікаве питання: Як ви важаєте, що є кориснішим в контексті дистанційно керованого апарату?

Прикладом позитивного зворотнього зв'язку в хімії є вибух, тобто бомба =). [3.1.3.][3.1.3.]

### Пропорційно-інтегрально-диференціальний закон регулювання

**(ПІД) регулятор** — це механізм керування із зворотним зв’язком, який широко використовується для
управління обладнанням і процесами, що потребують безперервного контролю та автоматичного регулювання. [3.1.1.1.][3.1.1.1.]

Простим прикладом циклу управління є налаштування необхідної температури води
при заповнені ємності за допомогою ручок крану, що дозволяють контролювати
змішування холодної та гарячої води. Людина дотиком перевіряє температуру води.
На основі цих відчуттів вона виконує дію повертаючи холодний чи гарячий кран,
доки не встановить необхідну температуру води в ємності. [3.1.1.2.][3.1.1.2.]

Для дронів це може бути механізм, який дозволяє тримати їхню рівновагу в повітрі. [FPV Drone PID Explained](https://oscarliang.com/pid/)

## Дистанційне керування

**Дистанці́йне керува́ння**, — керування об'єктами і системами на відстані шляхом передачі
до них каналами зв'язку сигналів для увімкнення відповідних виконавчих пристроїв
(реле, вимикачів, контакторів, пускачів, вентилів, засувок тощо). [3.2.1.][3.2.1.]

### ArduPilot/Mission Planner/MAVLink

#### ArduPilot
**ArduPilot** is a trusted, versatile, and open source autopilot system supporting
many vehicle types: multi-copters, traditional helicopters, fixed wing aircraft,
boats, submarines, rovers and more. [сайт](https://ardupilot.org/)

#### Mission Planner
**Mission Planner** is a full-featured ground station application
for the ArduPilot open source autopilot project.

It is a ground control station (GCS) for Plane, Copter and Rover. [сайт](https://ardupilot.org/planner/docs/mission-planner-overview.html) 

A ground control system (GCS) is a collection of hardware and software
tools that enable operators to remotely control and monitor unmanned aerial systems (UAS) from the ground. [3.2.1.2.1][3.2.1.2.1]

#### MAVLink

**MAVLink (англ. Micro Air Vehicle Link)** — комунікаційний протокол безпілотного апарату із наземною станцією. [3.2.1.3.1][3.2.1.3.1]


## Штучний інтелект

### Алгоритм пошуку A*
https://www.reddit.com/r/computerscience/comments/t8hdut/is_pathfinding_considered_artificial_intelligence/
https://www.statsig.com/perspectives/pathfinder-userflows-aipathfinding
https://en.wikipedia.org/wiki/A*_search_algorithm
https://en.wikipedia.org/wiki/Pathfinding#A*_algorithm


## Джерела

[3.1.]: https://uk.wikipedia.org/wiki/%D0%A0%D0%BE%D0%B1%D0%BE%D1%82%D0%BE%D1%82%D0%B5%D1%85%D0%BD%D1%96%D0%BA%D0%B0

[3.1.1.]: https://uk.wikipedia.org/wiki/%D0%97%D0%B2%D0%BE%D1%80%D0%BE%D1%82%D0%BD%D0%B8%D0%B9_%D0%B7%D0%B2%27%D1%8F%D0%B7%D0%BE%D0%BA

[3.1.2.]: https://en.wikipedia.org/wiki/Negative_feedback

[3.1.3.]: https://en.wikipedia.org/wiki/Positive_feedback

[3.1.1.1.]: https://en.wikipedia.org/wiki/PID_controller

[3.1.1.2.]: https://uk.wikipedia.org/wiki/%D0%9F%D1%80%D0%BE%D0%BF%D0%BE%D1%80%D1%86%D1%96%D0%B9%D0%BD%D0%BE-%D1%96%D0%BD%D1%82%D0%B5%D0%B3%D1%80%D0%B0%D0%BB%D1%8C%D0%BD%D0%BE-%D0%B4%D0%B8%D1%84%D0%B5%D1%80%D0%B5%D0%BD%D1%86%D1%96%D0%B0%D0%BB%D1%8C%D0%BD%D0%B8%D0%B9_%D0%B7%D0%B0%D0%BA%D0%BE%D0%BD_%D1%80%D0%B5%D0%B3%D1%83%D0%BB%D1%8E%D0%B2%D0%B0%D0%BD%D0%BD%D1%8F

[3.2.1.]: https://uk.wikipedia.org/wiki/%D0%94%D0%B8%D1%81%D1%82%D0%B0%D0%BD%D1%86%D1%96%D0%B9%D0%BD%D0%B5_%D0%BA%D0%B5%D1%80%D1%83%D0%B2%D0%B0%D0%BD%D0%BD%D1%8F

[3.2.1.2.1]: https://www.telecomtrainer.com/gcs-ground-control-system/

[3.2.1.3.1]: https://uk.wikipedia.org/wiki/MAVLink
