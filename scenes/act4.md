# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (игра сохранена)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *вздох*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Какова, чёрт возьми, мораль этой истории?

`hong({body:"one_up", eyes:"annoyed"})`

h: Что мы вообще *узнали*? Я был *глуп*, мои "друзья" *использовали* меня, и мы чуть не *погибли*.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Да, не говоря уже о больничном счёте.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Да, не говоря уже об уроне печени.](#act4a_liver)
{{/if}}

[Да, это *был* худший сценарий.](#act4a_worst)

[Да, я был прав.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Верно. Я не думаю, что моя страховка покрывает "быть тупым идиотом".

`hong({eyes:"annoyed", mouth:"normal"});`

b: И, всё же... мы выжили!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Мы определенно сбросили несколько лет от ожидаемой продолжительности жизни...

`bb({eyes:"surprise"});`

b: Но, по крайней мере, у нас *всё ещё* есть ожидаемая продолжительность жизни! Мы выжили!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: И, всё же...

h: Хм?

`bb({eyes:"surprise"});`

b: Мы выжили!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Но... ты тоже прав.

`hong({eyes:"surprise"});`

h: Хм?

`bb({eyes:"normal"});`

b: Я *был* волком что кричал "волки". Поэтому, когда появилась *реальная* опасность, ты - по праву - не поверил мне.

`bb({eyes:"surprise_r"});`

b: И, всё же, мы выжили!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Несмотря ни на что, мы всё ещё здесь.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: Ты кажешься довольно спокойным, учитывая, что у нас только что был опыт смерти.
{{/if}}

{{if !_.INJURED}}
h: Ты выглядишь довольно спокойным, учитывая, что у нас только что был предсмертный опыт.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Ну, это делает всё остальное менее страшным в сравнении. Это также заставило меня задуматься.

`bb({eyes:"normal", mouth:"normal"});`

b: Если мы сражаемся, то ты проигрываешь, потому это не защищает тебя...

h: Но когда мы сражаемся, то ты *тоже* проигрываешь, потому что это просто заставляет тебя кричать громче...

`bb({eyes:"normal_r"})`

b: Тогда, может быть...

`bb({eyes:"normal"})`

h: Может мы не должны сражаться.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: Я не Большой Плохой Волк. Но я и не сторожевой волк тоже.

`bb({eyes:"sad_d"})`

b: Я побитая приёмная собака.

`bb({eyes:"sad"})`

b: Мы прошли через трудные времена. Может быть, травму или пренебрежение. Вот почему я иногда слишком остро реагирую и говорю:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: ТЯФ ТЯФ ТЯФ ТЯФ ТЯФ

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Но я *не хочу* быть трусливой собакой! Я хочу защищать тебя! Я хочу быть хорошей собакой!

`bb({eyes:"sad", mouth:"normal"});`

b: Человек... ты поможешь приручить этого волка?

`hong({eyes:"sad"})`

h: Я... Я попробую.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Окей. Здоровые отношения с эмоциями. Отношениям нужна коммуникация. Так что, давай коммуницировать.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: Следующие пять минут будут казаться супер стрёмными, но давай притворяться, пока мы не сделаем это.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Дорогой внутренний волк... как *ты* себя чувствуешь?

n2: ИСПОЛЬЗОВАННЫЕ СТРАХИ:

n2: *ВРЕД* {{_.attack_harm_total}}, *НЕЛЮБОВЬ* {{_.attack_alone_total}}, *РЕПУТАЦИЯ* {{_.attack_bad_total}}

n2: О КАКОМ СТРАХЕ ТЫ ХОЧЕШЬ ПОГОВОРИТЬ В ПЕРВУЮ ОЧЕРЕДЬ? (ТЫ СМОЖЕШЬ ВЫБРАТЬ ДРУГИЕ ПОЗЖЕ)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Я боюсь что нам навредят.](#act4_harm)

[Я боюсь, что мы останемся одинокими.](#act4_alone)

[Я боюсь, что мы плохие люди.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Я хочу защитить твою потребность в физической безопасности,

`bb({eyes:"sad_d"})`

b: Но *весь мир* кажется таким опасным. Так много трагедий и зла.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: Я не знаю, достаточно того, что *я* выбираю, что сказать дальше. Что *ты* скажешь, человек?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: И снова, возвращаясь к тебе, человек. Что ты думаешь?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Ещё мысли, человек?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Ты прав. Давай защищаться.](#act4_harm_skills)

[Давайте подвергнем себя ещё *большей* опасности.](#act4_harm_exposure)

[Спасибо.](#act4_thanks) `_.thanks_for = "физической безопасности";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Но... как? У меня есть клыки и когти, но я всего лишь метафора.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Мы могли бы научиться самообороне? Присоединиться к сообществам, которые защищают друг друга?

h: Улучшить наше общее состояние здоровья и личные границы?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Может быть, но...

[С чего мы вообще начнём?](#act4_harm_skills_start)

[Что, если они всё ещё не работают?](#act4_harm_skills_work)

[Что, если мы переборщим с "безопасностью"?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: Так много нужно сделать, так много мы должны исправить в себе. Когда мы вообще *начнём*?

`hong({ body:"shrug", eyes:"surprise" })`

h: Мы начинаем прямо сейчас.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Ээ?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Сейчас мы практикуем хорошее общение. Что поможет нам обнаруживать опасность лучше, с меньшим числом ложных срабатываний,

`hong({ eyes:"surprise" });`

h: И *это* поможет защитить нас от увечий!

`hong({ eyes:"normal", mouth:"normal" });`

h: Поэтому: *это* обучение самообороне.

`bb({ eyes:"normal_r" })`

b: Хах. Я больше ожидал что-то такого:

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: Правда, способа защитить себя на 100% не существует...

`hong({ body:"one_up" });`

h: Но даже прогресс в 1% уже стоит того, верно?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Ты видишь стакан не на 99% пустым, а на 1% полным?

`bb({ eyes:"normal" });`

h: Что всё ещё имеет ценность, если ты застрял в пустыне.

`bb({ eyes:"closed" });`

b: Что ж. Тогда пей до дна.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Я имею в виду, причина, по которой ты игнорировал мои предупреждения, была в том, что я переборщил с безопасностью!

`bb({ body:"normal", eyes:"normal" })`

h: Не, ты прав. Мы хотим сделать умеренную безопасность. Всё в меру.

`bb({ eyes:"suspect" })`

b: Прости, *ВСЁ* в меру?

`hong({ eyes:"annoyed" })`

h: *Умеренное число вещей* в меру.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Спасибо, что сделал свои утверждения рекурсивно самосогласованными.

(#act4_something_else)

# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *ЧТО*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Ну, скажем, собака боится грома.

`hong({ body:"hands_1" });`

h: Дрессировщики используют один трюк, они проигрывают запись грома на низкой громкости,

h: а затем дают собаке лакомство для сохранения спокойствия.

`hong({ body:"hands_2" });`

h: В течение нескольких дней дрессировщик постепенно повышает громкость, пока собака не преодолеет свой страх перед громом.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Это называется экспозиционной терапией!

`hong({ body:"point", eyes:"normal" });`

h: Поскольку ты собака, это должно сработать и для тебя, верно? У всех млекопитающих одинаковая реакция "борись или беги".

`hong({ body:"normal" });`

[Что делать, если мы *слишком* десенсибилизируем?](#act4_harm_exposure_overboard)

[Что, если мы подвергнемся *реальной* опасности?](#act4_harm_exposure_hurt)

[Я волк, а не собака.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: И я буду проявлять к тебе доброту и терпение, пока ты не превратишься в милого маленького щенка.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Ооо.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: Мы *просто* видели, что происходит, если ты закрываешь свой страх – ты ставишь себя в *действительно* опасные ситуации.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Кроме того, разве *слишком* сильная десенсибилизация не превратит нас в психопатов?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Скоро мы будем вознаграждать себя во время просмотра убийственных снафф порно!

`hong({ eyes:"annoyed" })`

h: Я... думаю, между этим и громом всё же есть граница.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Но *где* именно, человек? *Где?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: Я не знаю. Но *ты* можешь мне помочь!

`hong({ eyes:"normal", body:"normal" })`

h: Работая и ведя переговоры с тобой, мы проведём эту линию.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Окей. Но у меня нет больших пальцев, так что ты должен сделать рисунок.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: Например: мы спрыгнули с чёртовой *крыши!*
{{/if}}

{{if !_.INJURED}}
b: Например: мы почти что спрыгнули с чёртовой *крыши!*
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Не, ты прав. Один из нас *может* зайти слишком далеко.

`hong({ eyes:"normal" });`

h: Но именно поэтому, если мы будем проводить экспозиционную терапию, то начнём с малого и будем делать маленькие шаги вперёд.

h: Как раз, когда мы столкнёмся с *реальной* опасностью, мы остановимся.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Да, я провожу черту между слышаньем громкого грома, и стоянием в буре с высокой остроконечной шляпой.

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: Подожди, никаких аргументов за или против того что я чувствую? Просто... "спасибо"?

`hong({ eyes:"surprise", body:"shrug" })`

h: Да! Спасибо, что проявил свою заботу о моей {{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Ты в порядке?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Ты никогда прежде не говорил мне *спасибо*.

`hong({ mouth:"smile" });`

h: Ооо ты большой мягкий-тёплый волк-паникёр.

(#act4_something_else)

# act4_thanks_2

h: Даже если ты слишком остро реагируешь, я ценю, что ты заботишься о моей {{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: Погоди... ты ведь не просто повторяешь "Спасибо", чтобы на самом деле не говорить об этих страхах, не так ли?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Ну, всё сложно, и у меня не всегда есть готовые ответы.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Это не похоже на то, что жизнь даёт тебе список из 3-х готовых диалоговых ответов.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Но сейчас, по крайней мере, я могу хотя бы сказать спасибо.

b: Что ж, спасибо и тебе, что терпеливо меня выслушал.

`bb({ eyes:"closed" });`

b: Ты маленький, безволосый, кожный млекопитающий.

(#act4_something_else)

# act4_thanks_3

h: Даже если твоё тявканье пугает меня, ты просто пытаешься защитить мою {{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: Так, если ты и дальше будешь так мне льстить, в интернете появятся странные идеи о нас.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Да ладно, я просто уязвимый ребёнок студенческого возраста, а ты большой, страшный волк. Что плохого может--

`hong({ eyes:"normal", body:"point" });`

h: Правда, не отвечай на это.

(#act4_something_else)

# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Я хочу убедиться, что ты удовлетворяешь эту глубокую, человеческую потребность в принадлежности...

`bb({ eyes:"sad_u" });`

b: Но я беспокоюсь, что если кто-нибудь когда-нибудь узнает нас *настоящих* - мы отпугнем их всех.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Я не знаю, достаточно того, что *я* выбираю, что сказать дальше. Что *ты* скажешь, человек?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: И снова, возвращаясь к тебе, человек. Что ты думаешь?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Ещё мысли, человек?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Я согласен: поработаем с нашей социальной жизнью.](#act4_alone_skills)

[Я думаю мы нравимся людям. Давай выясним?](#act4_alone_experiment)

[Спасибо.](#act4_thanks) `_.thanks_for = "социальной принадлежности";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Мы могли бы практиковать такие навыки, как задавать вопросы, слушать и сопереживать, быть открытыми и уязвимыми и т.д.?

`hong({ eyes:"normal_l" });`

h: Или сделать лучше социальные привычки, как планирование времени с друзьями или регулярные знакомства?

`hong({ body:"one_up" });`

h: Можно также научиться чувствовать себя более комфортно с отказами.

`hong({ eyes:"normal" });`

h: Или научиться знать, когда люди *не* отвергают нас, потому что они просто устали или имеют Синдром Стервозного Лица.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Много вариантов. Но, говоря об "изучении социальных навыков"...

[Это не *манипуляция?*](#act4_alone_skills_manipulative)

[Это не делает нас *уязвимыми для манипуляций?*](#act4_alone_skills_manipulated)

[Что, если мы всё равно потерпим неудачу?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Разве серийные убийцы, умеющие читать эмоции своих жертв, не умеют "сопереживать"?

`bb({ eyes:"annoyed" });`

b: Разве Чарльз Мэнсон не завоёвывал друзей и не влиял на людей?

`hong({ eyes:"annoyed", body:"chin" });`

h: Нет, ты прав.

h: "Социальные навыки" ничего не значат, если мы действительно не заботимся *о* людях.

`hong({ body:"normal" });`

h: Проще говоря, просто не будь мудаком.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Это мотивационный заголовок плаката прямо вон там.

`hong({ body:"shrug", mouth:"narrow" });`

h: "Не будь мудаком™"

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Мы станем желанным ковриком, говоря "Пожалуйста" и "Спасибо", когда люди вытирают о нас ноги!

`bb({ mouth:"scream", eyes:"scream" })`

b: Мы будем целовать так много задниц, что это будет выглядеть так, будто мы носим коричневую помаду!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Ох, ты прав. "Социальные навыки" не могут быть просто о том, чтобы угождать другим, они также об установке *границ.*

`hong( body:"one_up" });`

h: Мы не можем приглашать других в наш дом, если у нас нет стен, чтобы поддержать наш дом.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: Кстати... re: тот мысленный образ губной помады... *фу??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Мы можем потерпеть неудачу. На самом деле, мы *потерпим* неудачу.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: И это прекрасно! Неудача - это то, как начать узнавать что-то новое!

`hong({ body:"normal", eyes:"normal" });`

h: Так что давайте двигаться вперед вместе, хорошо?

`bb({ eyes:"normal_r" });`

b: Конечно, я согласен... в худшем случае, мы можем просто сбежать из города и создать новую личность.

`bb({ eyes:"normal" });`

h: Да, я думаю, сейчас это стоит около двух биткоинов.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Мы могли бы попробовать некоторые эксперименты!

`hong({ body:"chin" });`

h: Мы могли бы связаться с другом, чтобы пообщаться, восстановить связь со старым приятелем или даже просто пообщаться с бариста.

`hong({ body:"normal" });`

h: Думаю, мы обнаружим, что мы более привлекательны, чем думаем.

`bb({ eyes:"annoyed" });`

[Что, если это маленькие, дешёвые "победы"?](#act4_alone_experiment_cheap)

[Что, если это бремя для других?](#act4_alone_experiment_burden)

[Но светская беседа это ещё не *настоящие* мы!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Если мы нацепим на себя фальшивую улыбку, то мы никогда ни с кем не свяжемся по-настоящему,

`bb({ eyes:"super_sad" });`

b: *Но* если мы откроемся, то другие люди увидят все наши испорченные внутренности!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Перевернись.

b: Что.

`hong({body:"hands_1"})`

h: Когда собаки хотят показать свою любовь и доверие, они делают себя уязвимыми, обнажая свой живот.

`hong({body:"one_up"})`

h: Может быть, мы *ещё* недостаточно защищены, чтобы быть слишком уязвимыми, но хорошо потренировавшись,

`hong({body:"normal", eyes:"surprise"})`

h: Когда-нибудь мы сможем показать людям настоящих нас – полностью испорченных, но всем людям.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Я перевернусь если ты дашь мне вкусняшку.

`bb({ eyes:"normal", mouth:"normal" });`

h: Нет.

(#act4_something_else)

# act4_alone_experiment_cheap

b: Сказать "Привет" баристе это не совсем выступление с золотой медалью на Социальной Сетевой Олимпиаде.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Это для *нас!*

`hong({ body:"one_up", eyes:"annoyed" });`

h: На социальной арене мы даже не в полулегком весе, мы такие... кварк-вес.

`hong({ body:"normal", eyes:"normal" });`

h: Если мы должны начать с маленьких, дешёвых побед, то так тому и быть. Нужно подниматься с 1-го до 1000-го шага.

b: Да! Может быть, сказав "Привет", мы сможем перейти к разговору...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Как ты?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Не очень!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Может быть, бариста просто хочет сделать какой-нибудь чёртов кофе,

b: а не быть *экспериментом* и видеть насколько плохи наши социальные навыки.

`bb({ eyes:"annoyed" })`

h: Ну, если окажется, что мы *являемся* обузой...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Это тоже хорошо знать!

`hong({ eyes:"normal" });`

h: Так мы сможем научиться активно расспрашивать людей об их комфорте, знать и уважать границы других.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Знаешь, все эти ^дерьмовые^ "межличностные навыки" что мы видим в брошюрах консультантов.

(#act4_something_else)

# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Я хочу защитить твои моральные потребности, то стремление стать лучшим человеком,

`bb({ eyes:"sad_d" })`

b: Но мне просто кажется, что в глубине души мы фундаментально... сломаны.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: И не говори мне, что мы *не* запутаны. Мы спрыгнули с *крыши*.
{{/if}}

{{if !_.INJURED}}
b: И не говори мне, что мы *не* запутаны. Мы чуть не спрыгнули с *крыши*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: Не знаю, достаточно того, что *я* выбираю, что сказать дальше. Что *ты* скажешь, человек?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: И снова, возвращаясь к тебе, человек. Что ты думаешь?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Ещё мысли, человек?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Что ж, мы сломаны. Давай исправим нас.](#act4_bad_fix)

[Что ж, мы сломаны. Давай примем это.](#act4_bad_accept)

[Спасибо.](#act4_thanks) `_.thanks_for = "моральном благополучии";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Мы могли бы постепенно выработать лучшие привычки, привести нашу жизнь в соответствие с тем, что мы ценим,

`hong({body:"one_up"});`

h: А при необходимости мы могли бы получить профессиональную помощь терапевта или консультанта.

`hong({body:"normal"});`

h: Есть способы нас исправить.

[Что, если мы не сможем все исправить?](#act4_bad_fix_cant)

[Что делать, если мы *слишком* десенсибилизируем?](#act4_bad_fix_too_much)

[Мы не можем позволить профессиональную помощь.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Не, наверное ты прав.

h: Мы не можем исправить всё.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ах, я знал, что мы всегда будем сломаны!

`hong({eyes:"surprise"});`

h: Но, по крайней мере, мы можем быть *менее* сломанными.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Шрамы со временем заживают, но никогда не исчезают. И это нормально.

`bb({eyes:"annoyed_r"});`

b: Согласен. Кроме того,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Шрамы *сексуальны.*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Пожалуйста не делай этого.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Это неприятно признавать, но... какая-то часть меня *хочет* иметь это расстройство.

`bb({ eyes:"angry" })`

b: Я имею ввиду, без него, мы не станем *скучными?*

`bb({ eyes:"sad_r", body:"one_up" })`

b: Без расстройства мы не станем чёрствыми и пресными?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Без расстройства мы не сможем связаться с нашими друзьями, у которых тоже есть это расстройство?

`bb({ eyes:"sad", body:"chest" })`

b: Если мы когда-нибудь будем довольны жизнью, не перестанем ли мы заставлять себя делать великие дела?

`hong({ MOUTH_LOCK:true })`

h: ...

h: Если мы даже боимся... "избегать страхов"...

h: Я не думаю, что у нас закончатся страхи.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Ох, да! Фух! Какое облегчение!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Док, я беспокоюсь, что я плачу $100/час только для того, чтобы услышать, как вы спрашиваете *как вы себя чувствуете?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Мм-хмм. И как вы себя при этом чувствуете?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Не, это вполне обоснованное беспокойство.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: И это действительно отстой, что психомедицина не доступна для многих людей.

`hong({ eyes:"normal", mouth:"normal" });`

h: Тем не менее, есть несколько дешёвых или бесплатных вариантов:

`hong({ body:"chin" })`

h: Группы поддержки, онлайн-терапия, студенческие/некоммерческие центры здоровья...

`hong({ body:"hands_1" })`

h: Формирование привычек, таких как медитация, хороший сон, регулярное общение с друзьями, изучение новых вещей...

`hong({ body:"hands_2" })`

h: Походы в библиотеку, чтобы взять книги доказательной психотерапии...

`hong({ body:"one_up" })`

h: В конце игры есть полный список ресурсов об этом!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Что ж, *эта* четвёртая стена продержалась недолго.

`hong({ body:"point" });`

h: Некоторые вещи более важны, чем нарративные конвенции. Как, например, психическое здоровье.

(#act4_something_else)

# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Я имею в виду, это то, что говорят терапевты, верно? Принять все свои эмоции, даже негативные?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Подожди.

["Принять" как *сдасться*?](#act4_bad_accept_give_up)

["Принять" как *позволить*?](#act4_bad_accept_approve)

["Принять" как *взять буквально*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Как думаешь, Мартин Лютер Кинг сказал бы: "чёрт, мы не можем сидеть в передней части автобуса, давайте просто *примем* это?"

`bb({ eyes:"angry_r", body:"two_up" });`

b: Почему Промышленный Комплекс Самопомощи думает, что размахивание белым флагом - это какая-то *глубокая мудрость?*

`bb({ eyes:"annoyed", body:"normal" });`

h: Я думаю, что терапевты имеют в виду "принять" плохие вещи, как есть: признавать их существование и трудность изменения,

h: Но не обязательно отказываться от обязательства измениться.

`bb({ eyes:"suspect" });`

b: Тогда терапевты должны говорить: *признать*, а не *принять*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Да, если подумать, "принять" немного запутывает.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Что ж, я *признаю* это.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Как будто это *хорошо*, что мы сломаны или что-то вроде? Нет!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Все эти чертовы голливудские сценаристы, которые романтизируют психические заболевания, полны грязи!

`bb({ eyes:"angry", body:"two_up" });`

b: Иметь психическое расстройства *отстой!* Они отнимают у людей *жизни!* Почему мы должны "принимать" это?!

`bb({ body:"normal" });`

h: Я думаю, что терапевты имеют в виду "принимать" наши эмоции, как есть: быть терпеливым с ними.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Например, как борьба в зыбучих песках заставляет тебя тонуть быстрее и решение состоит в том, чтобы терпеливо лежать,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Борясь с тобой, моим страхом, заставляя меня спрыгнуть с крыши.
{{/if}}

{{if !_.INJURED}}
h: Борясь с тобой, моим страхом, почти заставляя меня спрыгнуть с крыши.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Вместо этого решение состоит в том, чтобы делать то, что мы делаем сейчас – не бороться, но быть терпеливым друг с другом.

`bb({ eyes:"annoyed" });`

b: Тогда они должны говорить *это* вместо какого-то проблемного слова как "принять".

`hong({ body:"chin", eyes:"annoyed" });`

h: Да, если подумать, "принять" - отстой.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: Я не принимаю "принять".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Но мы уже *знаем*, ты не должен понимать меня буквально!

`bb({ eyes:"sad_u", body:"two_up" });`

b: Вся *проблема* в том, что я хочу помочь тебе, но я не умею использовать слова для этого!

`bb({ eyes:"sad", body:"normal" });`

h: Думаю, терапевты имеют в виду "принять" свои эмоции как: "не бороться или игнорировать их."

`hong({ eyes:"surprise", body:"one_up" });`

h: Чтобы слушать тебя, работать *с* тобой, но не воспринимать буквально то, что ты говоришь, как 100% правду.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Тогда терапевты должны говорить *это*, вместо какого-то неопределенного запутанного слова вроде "принять".

`hong({ body:"chin", eyes:"annoyed" });`

h: Наверное, они тоже не умеют пользоваться словами.

(#act4_something_else)

# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Не важно, хочешь поговорить о чём-нибудь ещё?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: Так, есть ещё какая-нибудь тяжесть на сердце?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Я боюсь что нам навредят.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Я боюсь, что мы останемся одинокими.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Я боюсь, что мы плохие люди.](#act4_bad)
{{/if}}

[Не, я в порядке.](#act4c_prelude)

# act4_something_else_2

h: Окей, думаю сейчас мы обсудили все страхи.

b: Да, здесь всего три страха.

h: Ага, ровно три.

b: Удобно.

(#act4c)

# act4c_prelude

h: Хорошо поболтали, команда.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: Это не какая-то *игра*, ты знаешь.

`bb({eyes:"angry_d", body:"one_up"})`

b: Построение здоровых отношений с эмоциями не так-то просто, как нажатие кнопок на экране.

`bb({eyes:"sad", body:"normal"})`

b: *Сможем* ли мы действительно поладить?

b: *Сможем* ли мы работать вместе, как команда?

`hong({eyes:"sad", body:"one_up"})`

h: Что ж,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: И-извините...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: В-вы не против, если я посижу с вами за ланчем?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *Это* твой возлюбленный? Почему он сидит в одиночестве, как психованный серийный убийца?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Спрашивать своего возлюбленного можем ли мы составить ему компанию? Ты знаешь, какими *нуждающимся* мы звучим?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s:*Это* твой возлюбленный? Мы нарушили его покой и тишину! Мы такая обуза!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: Я- Я имею в виду- это, это нормально если нет, Я просто...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Погоди, не тебя ли я видел на вечеринке?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Да, конечно! Иди сюда.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Прости, сейчас мне нужно побыть одному.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Да, ты была на диване! На первой же вечеринке, куда я ходил...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Где я запаниковал и ударил хозяина вечеринки.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Где я запаниковал и убежал в слезах.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Погоди, человек, мы можем поставить её в неловкое положение.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ах, я не хочу ставить тебя в неловкое положение!

`publish("act4", ["hong_to_alshire",4]);`

h2: Просто вспомнил дружеское лицо, вот и всё.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: АААААА Я ТАК И ЗНАЛ! ОН ОПАСНЫЙ ПАНИЧЕСКИЙ ПСИХОПАТ!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: ААААА ПЕРВОЕ ВПЕЧАТЛЕНИЕ КОТОРОЕ МЫ СДЕЛАЛИ БЫЛО "СВИДЕТЕЛЬСТВО МОЕЙ ТРАВМЫ"! ЗНАЧИТ ОН НАС НЕНАВИДИТ!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: АААААА МЫ ЗАСТАВИЛИ КОГО-ТО ВСПОМНИТЬ ТРАВМИРУЮЩЕЕ СОБЫТИЕ. ОДНО НАШЕ ПРИСУТСТВИЕ ПРИЧИНЯЕТ БОЛЬ ДРУГИМ.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Погоди, человек, она кажется сбитой с толку.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ах, никакого давления, конечно!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Просто говорю, что ты можешь сесть здесь, если захочешь.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: МЫ *СЛИШКОМ* ДРУЖЕЛЮБНЫ! КАК СЕРИЙНЫЙ УБИЙЦА ТЕД БАНДИ!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: ОН ПРОСТО ВЕЖЛИВ! НИКТО В *ДЕЙСТВИТЕЛЬНОСТИ* НЕ ХОЧЕТ БЫТЬ С НАМИ!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: АААА МЫ ВСЕГДА ЗАСТАВЛЯЕМ ДРУГИХ ЧУВСТВОВАТЬ СЕБЯ НЕЛОВКО!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Погоди, человек, мы можем поставить их в неловкое положение.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ах, я не хотел быть грубым!

`publish("act4", ["hong_to_alshire", 6]);`

h2: Мне просто нужно время, чтобы переварить свои эмоции. Пожалуйста, не воспринимай это как личный отказ.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: КАКИЕ БОЛЬНЫЕ, ИЗВРАЩЕННЫЕ МЫСЛИ ОНИ ОБДУМЫВАЮТ?! КАКИЕ ТЁМНЫЕ ЖЕЛАНИЯ НАПОЛНЯЮТ СЕРДЦА ЭТИХ ПСИХОВ?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: НАС ОТВЕРГЛИ! МЫ НИКОГДА НЕ БУДЕМ ЛЮБИМЫ!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: МЫ ПРЕРВАЛИ ИХ ЭМОЦИОНАЛЬНУЮ ОБРАБОТКУ! ТЕПЕРЬ ОНИ БУДУТ ТРАВМИРОВАНЫ НАВСЕГДА, И ЭТО ВСЁ НАША ВИНА!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: БЕГИ БЕГИ БЕГИ БЕГИ БЕГИ БЕГИ БЕГИ БЕГИ БЕГИ БЕГИ БЕГИ БЕГИ

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: Ух. Это было странно. Интересно, что творилось у неё в голове.

`publish("act4", ["hong_closer", 2]);`

h: Не важно, о чём мы говорили?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Ух, я забыл? Что-то о командах и работе?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Они говорят, что ты должен "примириться" со своими эмоциями, как будто твои эмоции это *военные преступники*.

`publish("act4", ["bb_closer", 7]);`

b: Но я хочу, чтобы мы заключили нечто *большее*, чем просто мир! Я хочу, чтобы мы были *союзниками!*

`publish("act4", ["bb_closer", 3]);`

b: Я хочу быть хорошим сторожевым псом. Так же, как голод и жажда являются сигналами тревоги для твоих физических потребностей,

`publish("act4", ["bb_closer", 8]);`

b: Я хочу быть сигналом тревоги для твоих *психологических* потребностей – твоих потребностей в безопасности, принадлежности, доброте.

`publish("act4", ["bb_closer", 1]);`

b: Но... Я плохо справляюсь со своей работой, поэтому мне нужно, чтобы ты меня обучил.

`publish("act4", ["bb_closer", 4]);`

b: Я не "всегда верен" и не "всегда иррационален". Я просто... стараюсь изо всех сил. Так что, пожалуйста,

`publish("act4", ["bb_closer", 30]);`

b: Помоги мне помочь тебе!

`publish("act4", ["bb_closer", 6]);`

b: Хотя, обучение старой собаки новым трюкам *займёт* некоторое время. Может быть, *годы.*

`publish("act4", ["bb_closer", 3]);`

b: И иногда у меня случаются рецидивы, я возвращаюсь к своим старым привычкам.

`publish("act4", ["bb_closer", 2]);`

b: Я буду лаять на тени. Я буду пугать тебя словами. Я мог бы даже показывать тебе некоторые навязчивые образы... вещей.

`publish("act4", ["bb_closer", 9]);`

b: Прости меня! Я побитая приёмная собака! Избитые собаки иногда какают на твою кровать!

`publish("act4", ["bb_closer", 4]);`

b: Но если ты будешь терпелив со мной... и просто останешься и посидишь со мной...

`publish("act4", ["bb_closer", 8]);`

b: Быть может, ты сможешь приручить этого волка.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Хорошая собака.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Хороший человек.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: ААААА МЫ ВСЁ ЕЩЁ ЕДИМ В ОДИНОЧЕСТВЕ ПЯТНАДЦАТЬ СИГАРЕТ ААААА
{{/if}}

{{if _.parasite}}
b: ААААА ТЫ ВСЁ ЕЩЁ НЕПРОДУКТИВЕН ПОКА ЕШЬ МЫ СОЦИАЛЬНЫЕ ПАРАЗИТЫ ААААА
{{/if}}

{{if _.whitebread}}
b: ААААА МЫ ЕДИМ БОЛЬШЕ БЕЛОГО ХЛЕБА ААААА
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: ТЯФ ТЯФ ТЯФ ТЯФ ТЯФ

(#credits)
