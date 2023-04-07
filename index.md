---
layout: page
title: Пропущений семестр твого навчання компʼютерним наукам
nositetitle: true
---

Університетьскі курси навчають вас складним темам компʼютерних наук - від операційних систем до машинного навчання, однак є одна важлива тема, яку рідко викладають, натомість дають студентам на самостійне опрацювання: уміння працювати з власним інструментарієм. Ми навчимо вас, як приборкати командний рядок, використовувати потужний текстовий редактор, користуватися фішками системи контролю версій, та багато іншого!

Студенти витрачають сотні годин, послуговуючись цими інструментами протягом їхнього навчання (і тисячі годин протягом їх карʼєри), тож має сенс зробити цей досвід максимально легким і безперешкодним. Освоєння цих інструментів не тільки дозволяє вам витрачати менше часу на те, щоб примусити їх робити те, що ви хочете, але також дозволяє вирішувати задачі, які до того здавалися до неможливості складними.


Про мотивацію, яка стоїть за цим курсом, можна прочитати [тут](/about/).

# Список лекцій

<ul>
{% assign lectures = site['2020'] | sort: 'date' %}
{% for lecture in lectures %}
    {% if lecture.phony != true %}
        <li>
        <strong>{{ lecture.date | date: '%-m/%d/%y' }}</strong>:
        {% if lecture.ready %}
            <a href="{{ site.baseurl }}{{ lecture.url }}">{{ lecture.title }}</a>
        {% else %}
            {{ lecture.title }} {% if lecture.noclass %}[no class]{% endif %}
        {% endif %}
        </li>
    {% endif %}
{% endfor %}
</ul>

Записи лекцій доступні [на
YouTube](https://www.youtube.com/playlist?list=PLyzOVJj3bHQuloKGG59rS43e29ro7I57J).

# About the class

**Викладачі**: Цей курс співвикладають [Anish](https://www.anishathalye.com/), [Jon](https://thesquareplanet.com/) і [Jose](http://josejg.com/).<br>
**Питання**: Пишіть нам на [missing-semester@mit.edu](mailto:missing-semester@mit.edu).

# Поза межами MIT

Ми також поділилися цим курсом поза межами MIT в сподіваннях, що комусь можуть знадобитися ці матеріали. Пости і коментарі можна знайти на платформах:

 - [Hacker News](https://news.ycombinator.com/item?id=22226380)
 - [Lobsters](https://lobste.rs/s/ti1k98/missing_semester_your_cs_education_mit)
 - [/r/learnprogramming](https://www.reddit.com/r/learnprogramming/comments/eyagda/the_missing_semester_of_your_cs_education_mit/)
 - [/r/programming](https://www.reddit.com/r/programming/comments/eyagcd/the_missing_semester_of_your_cs_education_mit/)
 - [Twitter](https://twitter.com/jonhoo/status/1224383452591509507)
 - [YouTube](https://www.youtube.com/playlist?list=PLyzOVJj3bHQuloKGG59rS43e29ro7I57J)


# Переклади

- [Англійська (оригінальний курс)](https://missing.csail.mit.edu)
- [Китайська (Спрощена)](https://missing-semester-cn.github.io/)
- [Китайська (Традиційна)](https://missing-semester-zh-hant.github.io/)
- [Японська](https://missing-semester-jp.github.io/)
- [Корейська](https://missing-semester-kr.github.io/)
- [Португальска](https://missing-semester-pt.github.io/)
- [Російська](https://missing-semester-rus.github.io/)
- [Сербська](https://netboxify.com/missing-semester/)
- [Іспанська](https://missing-semester-esp.github.io/)
- [Турецька](https://missing-semester-tr.github.io/)
- [Вʼєтнамська](https://missing-semester-vn.github.io/)
- [Арабська](https://missing-semester-ar.github.io/)
- [Італійська](https://missing-semester-it.github.io/)

Примітка: це посилання на переклади спільноти (окрім оригінального курсу), ми їх не перевіряли. 

Якщо ви створили власний переклад конспекту до курсу, надсилайте нам 
[pull request](https://github.com/missing-semester/missing-semester/pulls), аби ми додали його до списку!

## Подяки

Ми вдячні Elaine Mello, Jim Cain, а також [MIT Open
Learning](https://openlearning.mit.edu/) за можливість записати відео лекцій; Anthony Zolnik і [MIT
AeroAstro](https://aeroastro.mit.edu/) за відеоапаратуру; Brandi Adams і
[MIT EECS](https://www.eecs.mit.edu/) за підтримку цього курсу.

---

<div class="small center">

<p><a href="https://github.com/chytalka/missing-semester-ukr">Вихідний код</a>.</p>
<p>Ліцензовано на умовах CC BY-NC-SA.</p>
<p>Умови внесення змін і перекладу можна переглянути <a href="{{ site.baseurl }}/license/">тут</a>.</p>
</div>
