Опис домашнього завдання

Python має дві вбудовані функції сортування: sorted і sort. Функції сортування
Python використовують Timsort — гібридний алгоритм сортування, що поєднує в собі
сортування злиттям і сортування вставками.

Порівняйте три алгоритми сортування: злиттям, вставками та Timsort за часом
виконання. Аналіз повинен бути підтверджений емпіричними даними, отриманими
шляхом тестування алгоритмів на різних наборах даних. Емпірично перевірте
теоретичні оцінки складності алгоритмів, наприклад, сортуванням на великих
масивах. Для заміру часу виконання алгоритмів використовуйте модуль timeit.

Покажіть, що поєднання сортування злиттям і сортування вставками робить алгоритм
Timsort набагато ефективнішим, і саме з цієї причини програмісти, в більшості
випадків, використовують вбудовані в Python алгоритми, а не кодують самі.
Зробіть висновки.

На основі наданих даних про час виконання алгоритмів сортування для різних типів
масивів можна зробити наступні висновки:

Merge Sort:

В часових замірах видно, що Merge Sort працює значно повільніше за Timsort
(алгоритм, який використовується у Python для sorted). Час виконання зростає
значно при збільшенні розміру масиву, що підтверджує лінійну складність у
найгіршому випадку для Merge Sort. Insertion Sort:

Insertion Sort:

показує швидшість на відсортованих або майже відсортованих масивах, але значно
сповільнюється на випадкових масивах та збільшується з ростом їх розміру. Це
через квадратичну складність Insertion Sort, що стає очевидним при обробці
великих об'ємів даних. Timsort (Python's sorted):

Timsort:

виявляється найшвидшим серед трьох алгоритмів на всіх типах масивів. Він
демонструє майже стабільний час виконання, навіть при збільшенні розміру масиву,
що свідчить про його лінійно-логарифмічну складність. Це підтверджує
ефективність Timsort, особливо в контексті реалізацій вбудованих функцій
сортування у мові Python.

Висновок: Тим, що Timsort поєднує в собі переваги сортування злиттям і
сортування вставками, він є значно більш ефективним на практиці для більшості
наборів даних, які зустрічаються в програмуванні. Вбудовані функції сортування
Python (такі як sorted) використовують саме Timsort з цієї причини.
