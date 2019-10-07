# act1

```
SceneSetup.act1();
```

(...300)

n: И ЭТО ТРЕВОГА ЧЕЛОВЕКА

n: _ТЫ_ ЭТА ТРЕВОГА

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}

# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Ох, эй! Мы снова вернулись сюда?

`hong({eyes:"0_neutral"})`

n: ТВОЯ РАБОТА - ЗАЩИЩАТЬ СВОЕГО ЧЕЛОВЕКА ОТ *ОПАСНОСТЕЙ*

`bb({eyes:"look", mouth:"small_lock"})`

n: ФАКТИЧЕСКИ, ПЕРЕПРОХОЖДЕНИЕ ИГРЫ СТАВИТ ЕГО *ПОД УГРОЗУ* ПРЯМО СЕЙЧАС

n: БЫСТРЕЕ, ПРЕДУПРЕДИ ЕГО!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Человек! Слушай, ты в опасности! Игрок...

[...собирается снова нас мучать!](#act1_replay_torture)

[...не нашёл альтернативной концовки!](#act1_replay_alternate)

[...получит лудонарративный диссонанс!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Он заставит нас свернуться в клубок и плакать!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Он заставит нас убить твой телефон и вызвать паническую атаку!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Он заставит нас *НЕ* бить хозяина вечеринки!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Он заставит нас ударить симпатичного анти-злодейского хозяина вечеринки!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Ну, по крайней мере, мы не спрыгнем с крыши в этот р--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: ОН ЗАСТАВИТ НАС СПРЫГНУТЬ С КРЫШИ.
{{/if}}

`bb({body:"fear"});`

b: ВСЕ ЭТИ НОВЫЕ УЖАСНЫЕ ВЕЩИ ПРОИЗОЙДУТ С НАМИ, И ТОГДА МЫ--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Конечно, история *в целом* та же, но каждая глава имеет две возможных концовки, плюс все варианты ветвящегося диалога--

`bb({body:"fear"});`

b: Игрок разочаруется, закроет эту вкладку браузера, удалит нашу программу, и тогда мы--

(#act1_replay_end)

# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Чёрт, что сейчас?

`bb({eyes:"normal"});`

b: Сюжет истории был о том, как ты можешь *ВЫБРАТЬ* построение здорового сотрудничества со своим страхом,

`bb({eyes:"normal_right"});`

b: Но перезапуск игры даст ту же историю, подразумевая, что твой *ВЫБОР* не имеет значения,

`bb({eyes:"narrow_eyebrow"});`

b: Таким образом, показывая противоречие между связью игры и механики,

`bb({eyes:"fear"});`

b: Таким образом, распутывая ткань этой повествовательной вселенной,

`bb({body:"fear"});`

b: И тогда мы--

(#act1_replay_end)

# act1_replay_end

`bb({body:"panic"})`

b: УМРЁЁЁЁЁЁЁЁЁЁЁЁЁЁЁЁЁМ

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: Окей, давай вернёмся в роль.

```
Game.clearText();
```

n4: (ПОЗВОЛЬ СЫГРАТЬ _ТВОЕЙ_ ТРЕВОЖНОСТИ БЛА БЛА ЧТО ГОВОРИТ ТЕБЕ _ТВОЙ_ СТРАХ БЛА БЛА НУ ТЫ ЗНАЕШЬ)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)

# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: О боже, мой волк вернулся. Фантаааааааастика.

`hong({eyes:"0_neutral"})`

n: ТВОЯ РАБОТА - ЗАЩИЩАТЬ СВОЕГО ЧЕЛОВЕКА ОТ *ОПАСНОСТЕЙ*

`bb({eyes:"look", mouth:"small_lock"})`

n: ФАКТИЧЕСКИ, ЭТОТ СЭНДВИЧ СТАВИТ ЕГО ПОД *УГРОЗУ* ПРЯМО СЕЙЧАС

n: БЫСТРЕЕ, ПРЕДУПРЕДИ ЕГО!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Человек! Слушай, мы в опасности! Опасность в том, что...

`bb({body:"squeeze"})`

n4: (ПОЗВОЛЬ СЫГРАТЬ _ТВОЕЙ_ ТРЕВОЖНОСТИ! ВЫБЕРИ, ЧТО ГОВОРИТ ТЕБЕ _ТВОЙ_ СТРАХ)

(#act1_normal_choice)

# act1_normal_choice

[Мы обедаем одни! Снова!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Мы не продуктивны, пока едим!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Этот белый хлеб плох для нас!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Разве ты не знаешь, что одиночество приводит к преждевременной смерти - точно так же, как курение 15 сигарет в день?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Эм, спасибо за цитирование твоих источников, но--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Это значит, что если мы не будем тусоваться с кем-нибудь *прямо сейчас*, то мы-

`bb({body:"panic"})`

b: УМРЁЁЁЁЁЁЁЁЁЁЁЁЁЁЁЁЁМ

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: ТЫ ИСПОЛЬЗОВАЛ *СТРАХ НЕЛЮБВИ*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Вытащи свой ноутбук и поработай прямо сейчас!

`hong({eyes:"0_annoyed"})`

h: Эм, я бы предпочёл не сорить крошками в свою клавиа--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Если мы не вносим вклад в развитие общества, то мы - его паразиты!

b: Общественное тело отправится к общественному врачу за лекарствами, чтобы убить его общественных паразитов и тогда мы--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: УМРЁЁЁЁЁЁЁЁЁЁЁЁЁЁЁЁЁМ

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: ТЫ ИСПОЛЬЗОВАЛ *СТРАХ ПЛОХОЙ РЕПУТАЦИИ*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Эти исследования были воспроизвед--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Обработанная пшеница повысит уровень сахара в крови, поэтому им придется ампутировать все наши конечности, и тогда мы-

`bb({body:"panic"})`

b: УМРЁЁЁЁЁЁЁЁЁЁЁЁЁЁЁЁЁМ

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: ТЫ ИСПОЛЬЗОВАЛ *СТРАХ ВРЕДА*

(#act1b)

# act1b

n: ЭТО СУПЕР ЭФФЕКТИВНО

`bb({mouth:"smile", eyes:"smile"});`

b: Видишь, человек? Я твой верный сторож-волк!

`bb({body:"pride_talk"});`

b: Доверься своей интуиции! Твои чувства всегда верны!

`bb({body:"pride"});`

n: ОПУСТИ УРОВЕНЬ ЭНЕРГИИ ТВОЕГО ЧЕЛОВЕКА ДО НУЛЯ

n: ЧТОБЫ ЗАЩИТИТЬ ЕГО ФИЗИЧЕСКИЕ + СОЦИАЛЬНЫЕ + МОРАЛЬНЫЕ НУЖДЫ, ТЫ МОЖЕШЬ ИСПОЛЬЗОВАТЬ:

n: СТРАХ *ВРЕДА* #harm#

n: СТРАХ *НЕЛЮБВИ* #alone#

n: И СТРАХ *ПЛОХОЙ РЕПУТАЦИИ* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (ПОДСКАЗКА: ВЫБИРАЙ ТО, ЧТО ЗАДЕВАЕТ ЛИЧНО ТВОИ ГЛУБОКИЕ, ТЁМНЫЕ СТРАХИ!)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: знаешь что, возможно, пришло время проверить мой телефон.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: ЗАЩИЩАЙ СВОЕГО ЧЕЛОВЕКА

n: ОТ МИРА. ОТ ДРУГИХ ЛЮДЕЙ. ОТ НЕГО САМОГО.

n: УДАЧИ

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: ПЕРВЫЙ РАУНД: *БОЙ!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Хах. Лента Facebook говорит, что в эти выходные будет вечеринка.

`bb({eyes:"uncertain"});`

b: Разве этот чудак не проводит вечеринки *каждые* выходные?

`bb({eyes:"uncertain_right"});`

b: Какую внутреннюю пустоту они пытаются заполнить? Они, скорее всего, совершенно не в себе!

`hong({eyes:"surprise"});`

h: Кстати, мне прислали приглашение?

`bb({eyes:"fear", mouth:"normal"});`

b: Что ж!

[Скажи да, или мы умрём от одиночества!](#act1c_loner)

[Скажи нет, там полно ядовитых наркотиков!](#act1c_drugs)

[Проигнорируй, мы портим все вечеринки.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Пятнадцать сигарет в день, человек! Пятнадцать!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: Тогда никто не появится на наших похоронах, они выбросят наш пепел в океан, нас проглотит кит,
{{/if}}

{{if !_.fifteencigs}}
b: и мы станем КИТОВЬЕЙ КАКАШКОЙ!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: Так что да, мы должны пойти на эту вечеринку!
{{/if}}

{{if _.parasite}}
b: Просто принеси ноутбук, чтобы мы могли делать свою работу, а не быть общественным паразитом.
{{/if}}

{{if _.whitebread}}
b: Пока они не подают БЕЛЫЙ ХЛЕБ
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: БОЖЕ. Если это заставит тебя заткнуться, ладно.

h: Я скажу да.

{{if _.whalepoop}}
b: Китовья какашка, человек! Китовья какашка!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: или даже хуже... БЕЛЫМ ХЛЕБОМ
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Мы проглотим столько мета и белого хлеба, что они не смогут поместить наш жирный труп в печь для кремации!
{{/if}}

{{if !_.whitebread}}
b: Мы проглотим так много наркоты, что гробовщик будет удивляться, как наше тело *уже* забальзамировалось!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Кроме того, мы не можем веселиться, нам нужно работать, иначе мы - ужасные общественные паразиты!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: БОЖЕ. Если это заставит тебя заткнуться, ладно.

h: Я скажу нет.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Всё, что мы делаем, так это плачем в углу о том, что одиночество смертельно так же, как и 15 сигарет в день.
{{/if}}

{{if _.parasite}}
b: Всё, что мы делаем на вечеринках, так это беспокоимся о продуктивности.
{{/if}}

{{if _.whitebread}}
b: Всё, что мы делаем, так это беспокоимся о том, как нездоровая пища может нас убить.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: интересно, почему.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Поэтому, если мы пойдём, то заставим их чувствовать себя плохо, но если мы отклоним их приглашение, то также заставим их чувствовать себя плохо!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: ВСЁ ЧТО МЫ ДЕЛАЕМ ЗАСТАВЛЯЕТ ЛЮДЕЙ ЧУВСТВОВАТЬ СЕБЯ ПЛОХО ПОЭТОМУ МЫ ДОЛЖНЫ ЧУВСТВОВАТЬ СЕБЯ ПЛОХО

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Ох. Если это заставит тебя заткнуться, ладно.

h: Я проигнорирую приглашение.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Не важно. Facebook - это слишком. Мне нужно что-нибудь поспокойнее, менее тревожное.

`hong({eyes:"neutral"});`

h: Что нового в Twitter?

`bb({eyes:"look"});`

[О нет, взгляни на эту ужасную историю в новостях!](#act1d_news)

[О нет, эти твиты на самом деле о *нас?*](#act1d_subtweet)

[Эй, GIF-ка с котиком, лакающим молочко](#act1d_milk)

# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Боже, будто весь мир в огне, не так ли?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Такое ощущение, что всему конец, как будто всё умирает, и мы обречены, и мы ничего не можем с этим поделать.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Давай ретвитнем эту историю!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Окей, я ретвитну это, пожалуйста, успокойся!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: К чёрту, загляну в Snapchat.

(#act1e)

# act1d_subtweet

`bb({eyes:"fear"});`

b: Это сабтвит! Подлый, подлый сабтвит!

`hong({eyes:"annoyed"});`

h: А что, если нет?

`bb({eyes:"narrow", mouth:"small"});`

b: но что, если они все говорят за нашей спиной 

h: Они н--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: ПРЯМО ЗА НАШЕЙ СПИНОЙ

`hong({eyes:"sad", mouth:"sad"});`

h: Я н--

`bb({eyes:"narrow", mouth:"small"});`

b: но *что, если*

h: С--

`bb({eyes:"narrow_eyebrow"});`

b: *что, если*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: о-КЕЙ, попробую Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Хех, да, это довольно мило, просто ретвитну это, я ду--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: КОШКИ НЕ ПЕРЕВАРИВАЮТ МОЛОКО, И МЫ - УЖАСНЫЕ ЛЮДИ, НАСЛАЖДАЮЩИЕСЯ НАСИЛИЕМ НАД ЖИВОТНЫМИ

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: о-КЕЙ, попробую Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Хах, фотки со вчерашней ночи. Так *вот* какие эти еженедельные вечеринки.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Уф, выглядит слишком многолюдно для моей тревожности.

h: Может, мне не следовало соглашаться на приглашение?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Поменять наш ответ? Как придурок?!](#act1e_yes_dontchange)

[Измени наш ответ! Слишком многолюдно!](#act1e_yes_changetono)

{{if _.subtweet}}
[Мда, они правда твитили о нас.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Погоди, мы ретвитнули без факт-чекинга.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Ты знаешь, что у нас и правда плохая осанка?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Они рассчитывали, что мы приедём, и теперь мы предаём их доверие? Ты хочешь умереть в одиночестве?!

{{if _.fifteencigs}}
b: ПЯТНАДЦАТЬ. СИГАРЕТ.
{{/if}}

{{if _.whalepoop}}
b: КИТОВЬЯ. КАКАШКА.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Заткнись заткнись я оставлю "да"!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Разве ты не знаешь о людских давках?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: В 2003 году в ночном клубе на Род-Айленде произошел пожар, и паника заставила толпу людей заблокировать выходы,

b: в результате 100 человек сгорели до смерти.

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ТЫ ХОЧЕШЬ ЧТОБЫ ЭТО СЛУЧИЛОСЬ С НАМИ-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: СКАЖИ НЕТ СКАЖИ НЕТ СКАЖИ НЕТ СКАЖИ НЕТ СКАЖИ НЕТ СКАЖИ НЕТ СКАЖИ Н-

```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Заткнись заткнись я изменю свой ответ на "нет"! Боже!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Хм... выглядит забавно.

h: Может, мне не следовало отказываться от приглашения?

`bb({mouth:"normal", eyes:"normal"});`

[Изменить свой ответ? Как мудак?!](#act1e_no_dontchange)

[Поменяй ответ! Не умирай одиноким!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Мда, они действительно нас обсуждают.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Подожди, мы ретвитнули без проверки фактов.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Ты знаешь, что у тебя действительно плохая осанка?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Все рассчитывали на нас!

b: ...оставить их в покое и позволить им устроить хорошую вечеринку без ужасного отвратительного {{if _.whitebread}}жующего-белый-хлеб{{/if}} мерзавца, как ты--


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Заткнись заткнись я оставлю "нет"!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Хроническое одиночество увеличивает уровень кортизола, а также риск сердечно-сосудистых заболеваний и инсульта!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: ПЯТНАДЦАТЬ. СИГАРЕТ.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Заткнись заткнись я изменю свой ответ на "да"! Боже!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Все наши проблемные твиты вернулись к нам!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Нас призовут к ответу, отвергнут и будут тащить на веревке верхом по информационной магистрали!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Почему ты лайкнул это?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Мы распространяем дезинформацию! Мы уничтожаем доверие к свободным СМИ!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Мы - причина, по которой фашизм возникнет из обломков демократии!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: Почему ты лайкнул это?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Хочешь иметь позвоночник в виде кренделя?! Хватит сутулиться за экраном!

```
bb({body:"meta"});
```

b: Тебя это тоже касается.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Почему ты лайкнул это?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Хм... выглядит забавно.

h: Может мне не стоило игнорировать приглашение?

`bb({mouth:"normal", eyes:"normal"});`

[Игнорируй, мы недостаточно хороши для вечеринок.](#act1e_ignore_continue)

[Действительно, скажи да.](#act1e_ignore_changetoyes)

[Действительно, скажи нет.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: Хотя это грубо игнорировать их, нет?

`bb({eyes:"normal_right"});`

b: Ну, другие люди всегда игнорируют *нас*, так что

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: давай ответим им тем же.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Ты... позволишь мне повеселиться?

b: Ну, я имею ввиду, одиночество *может* нас убить.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: Слишком многолюдно. Толпы опасны.

(#act1e_yes_changetono)

# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Без разницы. Новое уведомление Tinder.

`bb({eyes:"uncertain"})`

b: Что, это приложение для знакомств?

`hong({eyes:"annoyed"})`

h: Это не приложение для знакомств, просто способ узнать новых люд--

`bb({eyes:"narrow"})`

b: Это приложение для знакомств.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: О, у меня совпадение! Выглядит мило!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Пожалуйста, не испорти м--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: ОПАСНОСТЬ ОПАСНОСТЬ ОПАСНОСТЬ ОПАСНОСТЬ ОПАСНОСТЬ

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Мы будем *использованы* другими людьми.](#act1f_used_by_others)

[Мы просто *используем* других людей.](#act1f_using_others)

[ТЫ СОВПАЛА С СЕРИЙНЫМ УБИЙЦЕЙ](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Случайные знакомства могут заполнить дыру здесь,

b: но они никогда не смогут заполнить дыру...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *здесь*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Суть в том, что МЫ УМРЁМ В ОДИНОЧЕСТВЕ

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Ты думаешь, что гениталии других людей - это покемоны для нашей коллекции?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (заглавная тема покемонов)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ Я хочу быть ^шлюха^тистей-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Как никто другой-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Бёдра и ^жопы^, манящая грудь-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ с потными ^хуем^ и яйцами!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ ^ШЛЮХА^МОН! ПОЙМАЙ ИХ-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Суть в том, что мы - манипуляторы.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: Он заманит тебя в ловушку и принудительно откормит тебя белым хлебом, чтобы он мог носить твою кожу как костюм!
{{/if}}

{{if _.parasite}}
b: Он забьёт тебя таймером помодоро и скажет: "ТЫ ДОЛЖЕН БЫТЬ ПРОДУКТИВНЫМ, ТЫ ПАРАЗИТ"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Он разорвёт твоё тело на кровавое конфетти, превратит твои внутренности в гирлянды и намешает твою кровь в чаше для пунша!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Как тебе ТАКОЕ приглашение на вечеринку?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: я так плох в этой игре.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"одиночество убьёт нас"... {{/if}}
{{if _.parasite}}"мы социальные паразиты"... {{/if}}
{{if _.whitebread}}"не ешь это, оно нас убьёт"... {{/if}}
{{if _.subtweet}}"они говорят за нашими спинами"... {{/if}}
{{if _.badnews}}"мир в огне"... {{/if}}
{{if _.hookuphole}}"мы умрём в одиночестве"... {{/if}}
{{if _.serialkiller}}"он - серийный убийца"... {{/if}}
{{if _.catmilk}}"кошки не переваривают молоко"... {{/if}}
{{if _.pokemon}}отстойная пародийная песня... {{/if}}

h: я просто хочу жить своей жизнью.

h: я просто хочу освободиться от всей этой... боли.

`bb({eyes:"look_sad"});`

b: Эй... человек...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Всё будет хорошо.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Как твой верный сторож-волк, я всегда буду начеку и сделаю всё возможное, чтобы ты был в безопасности.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Я обещаю.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Последнее приложение. Instagram. Что там у тебя?

`hong({eyes:"sad"});`

h: Эм... больше снимков с вечеринки.

`hong({mouth:"sad"});`

h: Все выглядят такими счастливыми. Свободные от забот. Свободные от тревоги.

`hong({mouth:"anger"});`

h: Боже, почему я не могу быть, как они? Почему я не могу просто быть *нормальным?*

`bb({eyes:"normal_right"});`

b: Говоря о вечеринках, вспомни то приглашение. Вот моё ФИНАЛЬНОЕ решение:

`bb({eyes:"normal"});`

[Мы должны пойти.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Мы не должны идти.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Мы--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *^НАХУЙ^.*

`hong({body:"2_you"});`

h: ТЕБЯ.

(...500)

b: ч

(...1500)

`bb({eyes:"wat_2"});`

b: что?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Я скажу ДА этой вечеринке,

{{if _.act1g=="go"}}
h: НЕ потому что ты хочешь, а потому что *я* этого хочу.
{{/if}}

{{if _.act1g=="dont"}}
h: Именно ПОТОМУ, что ты не хочешь.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Ты НЕ контролируешь меня.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: А теперь извини, я съем этот вкуснейший сэндвич в этом ^блядском^ месте.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[ААААА МЫ УМРЁМ](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[ААААА ВСЕ НАС НЕНАВИДЯТ](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[ААААА МЫ УЖАСНЫЕ ЛЮДИ](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: ААААА МЫ УМРЁМ ААААААААААААА

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: ААААА ВСЕ НАС НЕНАВИДЯТ ААААААААААААА

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: ААААА МЫ УЖАСНЫЕ ЛЮДИ ААААААААААААА

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: ПОЗДРАВЛЯЕМ

(...500)

n: ТЫ УСПЕШНО ЗАЩИТИЛ ФИЗИЧЕСКИЕ + СОЦИАЛЬНЫЕ + МОРАЛЬНЫЕ НУЖДЫ СВОЕГО ЧЕЛОВЕКА

n: ПОСМОТРИ, КАК ОН ТЕБЕ БЛАГОДАРЕН!

(...500)

n: ТЕПЕРЬ, КОГДА ЭНЕРГИЯ НА НУЛЕ, ТЫ МОЖЕШЬ КОНТРОЛИРОВАТЬ ЕГО ДЕЙСТВИЯ

`bb({mouth:"smile", eyes:"normal"});`

n: ВЫБЕРИ СВОЁ ЗАВЕРШАЮЩЕЕ ДВИЖЕНИЕ

`bb({mouth:"small_lock", eyes:"fear"});`

n: *ДОБЕЙ ЕГО*

[{БОРЬБА: Наказать свой стрессовый телефон!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{ОТСТУПЛЕНИЕ: Свернуться в клубок и плакать!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Твой телефон заставляет тебя паниковать!

`bb({eyes:"anger"})`

b: Цукерберк и Ко перерабатывают твоё ментальное здоровье в деньги венчурных капиталистов!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Накажи свой телефон! Уничтожь его! Убей!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: УБЕЙ ЕГО УБЕЙ ЕГО УБЕЙ ЕГО УБЕЙ ЕГО УБЕЙ ЕГО УБЕЙ ЕГО УБЕЙ ЕГО УБЕЙ ЕГО УБЕЙ ЕГО УБЕЙ ЕГО УБЕЙ ЕГО УБЕЙ ЕГО УБЕЙ ЕГО УБЕЙ Е--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Весь мир полон опасностей!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Действуй как броненосец! Свернись в клубок для самообороны!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: СВЕРНИСЬ И ПЛАЧЬ СВЕРНИСЬ И ПЛАЧЬ СВЕРНИСЬ И ПЛАЧЬ СВЕРНИСЬ И ПЛАЧЬ СВЕРНИСЬ И ПЛАЧЬ СВЕРНИСЬ И ПЛ-- 

(#act1j)

# act1j

`SceneSetup.act1_outro()`
