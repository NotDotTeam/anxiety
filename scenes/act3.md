# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Твоё здоровье!

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *Ах*, это то, что нужно.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: Знаешь, чувак...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: А именно, нужно моим миндалевидным телам.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Ты напоминаешь мне о моей молодости. Тогда, когда меня тоже мучило животное в моей голове.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: Я так благодарен, что я могу заплатить вперёд и помочь тебе убить зверя так же, как я убила своего.

```
publish("act3",["roofhunter",2]);
```

r: Эй, по-быстрому: правда или дейст--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: ДЕЙСТВИЕ!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Хаха! Отлично.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Видишь тот голубенький бассейн там внизу?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Этот? Шестью этажами ниже?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Спрыгни туда.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Подожди, что?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: Зверь начал ныть, не так ли?

```
publish("act3",["roofhunter",23]);
```

r: *О неееет, это опасно, не дееееелай этого.*

```
publish("act3",["roofhunter",22]);
```

r: Но именно поэтому нам нужны смертельно опасные трюки!

r: Оторвись по-полной! Carpe diem! Нюхни кокса с ^жопы^ этой шлюхи, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: Покажи зверю, что нам абсолютно *^похуй^* на его скулёж! Прыгай!

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Эм, но иногда, эмм... у страха есть смысл...

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: Извини, но ты реально ведёшься на всю эту пропаганду, что чувствовать себя плохо - это *хорошо?*

```
publish("act3",["roofhunter",17]);
```

r: ^Придурки^, что управляют этим миром, приносят *остальным* тревогу и депрессию,

```
publish("act3",["roofhunter",18]);
```

r: потом говорят в TED Talks чтобы мы "приняли" быть в конец ^ёбанутыми^ и "обняли" этого садистского демона в наших головах!

```
publish("act3",["roofhunter",6]);
```

r: Чувак, я знаю, что *ты* знаешь, что твоё животное *вредит* таким, как мы. Оно *мучает* таких, как мы.

```
publish("act3",["roofhunter",19]);
```

r: Оно нам не друг. Оно - бешенное животное, которого нужно либо *усыпить*,

```
publish("act3",["roofhunter",20]);
```

r: Либо пустить *пулю в его череп*.

```
publish("act3",["roofhunter",27]);
```

r: Иначе ты позволишь ему победить.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: Нет. Неправда.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
    music('battle_dark_loop');
});
```

h2: Я не позволю ему победить.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: Да, ^бля^! Я в тебя верю, малыш! Прикончи его! <3

(#act3a)



# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: нет нет нет нет нет нет

n: В ЭТОЙ ГЛАВЕ ДВА ВОЗМОЖНЫХ ИСХОДА. ОДИН ИЗ НИХ *ОЧЕНЬ, ОЧЕНЬ ПЛОХОЙ*.

b: НЕТ НЕТ НЕТ НЕТ НЕТ НЕТ НЕТ НЕТ

n: ВЫБИРАЙ МУДРО. ЗАЩИТИ СВОЕГО ЧЕЛОВЕКА.

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAA

`bb({ mouth:"normal" });`

n: УДАЧИ.

```
Game.clearText();
bb({ eyes:"start" });
```

[Человек, ты взаправду можешь ПОГИБНУТЬ!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[Это глупо и саморазушительно!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Эти придурки тебе никакие не друзья!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Ч--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Э--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Э--

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Знаешь, этому можно было бы поверить... если бы это не происходило тысячи раз подряд.

h: Ты волк, который кричал про волка.

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`


# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Это тоже уже было.

b: человек, не надо...

`hong({ eyes:"look_right" });`

h: Ох, *прости*, Фарм-компания не одобряет мои народные средства.

h: Слыш, ^мудак^, у *всех* есть способы заткнуть тебя ^нахер^.

`hong({ body:"look_up", eyes:"look_up" });`

h: Некоторые с головой бросаются в работу.

`hong({ body:"look_down", eyes:"look_down" });`

h: Некоторые бросаются в секс, наркотики и обновление их лент Facebook.

`hong({ body:"normal", eyes:"look_right" });`

h: Некоторые бросаются в поиски партнёра.

`hong({ eyes:"angry" });`

h: Я собираюсь броситься в этот бассейн.

[Ты пьян и он ШЕСТЬЮ ЭТАЖАМИ НИЖЕ!](#act3_bad_1_harm)

[Чёрт подери, и так ты меня благодаришь?](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Хорошо, я признаю. Это моя вина.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Даже если ты приземлишься в воду, поверхностное натяжение сломает твои рёбра и даст сотрясение *в лучшем случае!*

h: Эх.

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Я уже видел такое видео на YouTube.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: Я- Прости, *благодаришь?*

`bb({ eyes:"angry" });`

b: Именно поэтому я и *существую*! Потому что вам, людям, нельзя доверить даже собственную защиту!

b: Я пытаюсь защитить твою тупую задницу всю свою жизнь, и сейчас ты просто п--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: хех.

`hong({ body:"laugh_2" })``

h: хахахаха

`hong({ body:"laugh_3" })``

h: АХАХАХАХА

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: Ох, ВАУ, это величайшее *^блять^* преуменьшение века!

`hong({ body:"yell_2" });`

h: Да, ты, чёртова куча кроваво-красного ^дерьма^! Это твой огромный ^проёб^!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Что-нибудь ещё, Капитан Очевидность?

[Но месть мне - это не решение!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Но в этот раз я *на самом деле* прав!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Я тебя обидел.](#act3_good_2a)

# act3_good_1_fail_revenge

b: Тебе нужно построить более здоровые отношения с эмоциями, вместо того, чтобы бросаться с ними в--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)



# act3_good_1_fail_harm

b: Пожалуйста, просто поставь бутылку и давай--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)




# act3_bad_2

`bb({ eyes:"sad" });`

b: пожалуйста... не надо...

h: Твоя шкала энергии практически на нуле, волк.

h: На твоём месте, я бы подобрал свои следующие слова очень тщательно.

`bb({ eyes:"normal" });`

[Хорошо. Мне надоело тебя защищать.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Всё это время я был прав.](#act3_bad_2_right)

[Извини.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_2_jump

b: Ну же, вперёд, прыгай. Посмотри, как мне всё равно.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Отлично. До дна!

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: НЕТ ПОДОЖДИ ЭТО ОБРАТНАЯ ПСИХОЛОГИЯ ТЕБЕ НУЖНО ДЕЛАТЬ ВСЁ *НЕ ТАК* КАК Я СКАЗ--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: Ты *подвергаешь* себя опасности. Твои так называемые друзья *используют* тебя. И ты *используешь* своих так называемых друзей.

`bb({ eyes:"sad" });`

b: Пожалуйста, человек... почему ты не веришь мне?!

h: Потому что ты никогда не верил в *меня*.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: У других сторожевых волков есть люди, которые действительно тратят время на их дрессировку, *учатся* работать вместе,

b: Вместо того, чтобы их ненавидеть за попытки защитить! Почему бы тебе прост--

`bb({ eyes:"normal" });`

h: Неправильный ответ.

(#act3_bad_3)



# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *"Единственное, чего нам следует бояться, - это самого страха."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Don't worry, be happy!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Все мудрецы всех времён говорили: негативные эмоции *плохие!*

`hong({ eyes:"less_angry" });`

h: Ага! Именно поэтому их называют *негативными!*

b: человек... пожалуйста...

`hong({ eyes:"normal" });`

h: Совсем недавно я говорил: "Мне просто хочется избавиться от всей этой боли."

h: Желание исполнено. Я больше не чувствую ни боли, ни страха, ни тревоги...

h: Я вообще больше ничего не чувствую.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Я так волновался, что кто-нибудь причинит тебе боль, что даже не понимал, что это *я* причинял тебе боль.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: НЕТ, Б^ЛЯТ^Ь.

`hong({ body:"yell_1" });`

h: ^ПИЗДЕЦ^, тебе действительно понадобилось столько времени, чтобы это наконец понять?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Мы могли бы избежать стольких проблем, ты, большой пушистый ^долбоёб^. Почему тебе это раньше в голову не пришло?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...ты *извиняешься.*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: Извиняешься *за что?*

(#act3_good_2q)


# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized)
{{/if}}


# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[Извини, что я был плохим защитником.](#act3_good_3_protector)

[Извини, что не уважал тебя.](#act3_good_3_respect)

[Извини.](#act3_good_4)

# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Извини, что у меня такой ужасный человек!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Извини, что не уважал тебя.](#act3_good_3_respect)

[Извини, что сделал тебе больно.](#act3_good_3_hurt)

# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: Это было моей обязанностью - защищать тебя от *реальной* опасности, но я всё лаял на машины и почтальона.

`bb({eyes:"sorry_up"});`

b: Лаял на тени. Лаял так много.

`bb({eyes:"sorry"});`

b: Вполне логично, что ты хочешь надеть намордник.

`bb({eyes:"sorry_down"});`

b: Извини.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: Я должен быть *твоим* преданным сторожевым псом, но я вёл себя так, словно тебе нужно подчиняться *мне*.

`bb({eyes:"sorry_up"});`

b: Есть разница между защитником и тюремным охранником, и я перешёл эту границу.

`bb({eyes:"sorry_down"});`

b: Извини.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Я был настолько одержим идеей защитить тебя от боли, что никогда не мог подумать, что *я* буду причинять тебе боль.

`bb({eyes:"sorry_up"});`

b: Я плохой пёс.

`bb({eyes:"sorry_down"});`

b: Извини.

(#act3_good_4)


# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: Мда, это, конечно, была глупая идея.

h: Это должно было тебя проучить, и, видимо, так и получилось.

h: Давай просто закончим этот раунд вничью, ладно?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Хорошо.

h: Хорошо.

n: *НИЧЬЯ*

`_.a3_ending = "walkaway";`

(#act3_end)









# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}






# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: О, *да ладно*. После всего того, что это животное сделало с тобой, ты просто *сдаёшься?*

r: В чём проблема, чувак? Ты *боишься*?

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Да.

h2: Я боюсь.

`publish('hong-next')`

h2: И это нормально!

`publish('hong-next')`

h2: Бояться - нормально.

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: Они только что заперли дверь?

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)




# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```
(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: нет...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: нет нет нет

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: НЕТ!

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
