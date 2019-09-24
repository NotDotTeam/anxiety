# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Ура!

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

h2: *Ха* прям в точку.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: Ты знаешь, малыш...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: Конкретно, точками являются моя левая и правая миндалина.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Ты напоминаешь мне себя, когда я был моложе. Раньше, когда меня мучило животное в моей голове.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: Я так благодарен, что отплачу тебе тем же и помогу убить зверя так же, как я убил своего.

```
publish("act3",["roofhunter",2]);
```

r: Эй, блиц-вопрос: правда или де--

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

r: Хаха! Хорошо.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Ок. Видишь тот детский бассейн там внизу?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: А? Шестью этажами ниже?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Прыгни в него.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Погоди, что?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: Животное начало ныть, не так ли?

```
publish("act3",["roofhunter",23]);
```

r: *О неееет, это опасно, не дееееелай этого.*

```
publish("act3",["roofhunter",22]);
```

r: Но именно для этого нам и нужны смертельно-острые ощущения! Отрывайся! Лови момент! Снюхай дорожку с ^жопы^ проститутки, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: Покажи этому животному, что мы не дадим два *^хуя^* его ^сучк^е! Прыгай.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Ух, но иногда, эм... страх имеет смысл...

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

r: Извини, ты влюбился в эту чушь, что чувствовать себя плохо - это *хорошо?*

```
publish("act3",["roofhunter",17]);
```

r: Удовольствие это противоположность боли. Таким ^блядск^им образом, ты можешь использовать удовольствие, чтобы бороться с болью!

```
publish("act3",["roofhunter",18]);
```

r: Как эти псевдобудисты Силиконовой долины не замечают этого ^говн^а?!

```
publish("act3",["roofhunter",6]);
```

r: Малыш, я знаю, что *ты* знаешь, что животное *причиняет боль* людям, подобных нам. Он *мучает* таких людей, как мы.

```
publish("act3",["roofhunter",19]);
```

r: Это не наш друг. Это бешеный зверь, которого нужно либо *усыпить*,

```
publish("act3",["roofhunter",20]);
```

r: Или пустить *пулю в его череп*.

```
publish("act3",["roofhunter",27]);
```

r: В противном случае ты позволишь ему победить.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: Нет. Ты не прав.

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

r: Да, ^бля^! Я верю в тебя, детка! Прикончи его! <3

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

b: не не не не не не

n: В ЭТОЙ ГЛАВЕ ДВЕ ВОЗМОЖНЫЕ КОНЦОВКИ. ОДНА ИЗ НИХ *ОЧЕНЬ, ОЧЕНЬ ПЛОХАЯ.*

b: НЕТ НЕТ НЕТ НЕТ НЕТ НЕТ НЕТ НЕТ НЕТ НЕТ

n: ВЫБИРАЙ С УМОМ. ЗАЩИТИ СВОЕГО ЧЕЛОВЕКА

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: АААААААААААААААААА

`bb({ mouth:"normal" });`

n: УДАЧИ

```
Game.clearText();
bb({ eyes:"start" });
```

[Человек, ты правда можешь ПОГИБНУТЬ здесь!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[Это тупо и деструктивно!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Эти пьяницы не твои друзья!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

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

h: Знаешь, я бы тебе поверил... если бы ты не пробовал это миллион раз до этого.

h: Ты волк, который кричал "Волки!".

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

h: Это ты тоже пробовал.

b: человек, пожалуйста...

`hong({ eyes:"look_right" });`

h: Ой, *прости*, Big Pharma не одобряет моё самолечение.

h: Смотри ^уёбок^, у нас *всех* есть способ заткнуть тебя.

`hong({ body:"look_up", eyes:"look_up" });`

h: Некоторые люди бросают себя в работу.

`hong({ body:"look_down", eyes:"look_down" });`

h: Некоторые люди бросают себя в секс, наркотики и обновления их лент в Facebook.

`hong({ body:"normal", eyes:"look_right" });`

h: Некоторые люди кидают себя в других людей. 

`hong({ eyes:"angry" });`

h: Я же собираюсь бросить себя в тот бассейн.

[Ты пьян и здесь ШЕСТЬ ЭТАЖЕЙ ВНИЗ](#act3_bad_1_harm)

[Чёрт, это та благодарность, что я получаю?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Окей, я признаю это. Я напортачил.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Даже если ты окажешься в воде, поверхностное натяжение сломает твои рёбра и, как минимум, даст *сотрясение мозга!*

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

h: Я видел как русский чувак однажды сделал это на YouTube.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: Я- Прости, *благодарность?*

`bb({ eyes:"angry" });`

b: Именно поэтому я *существую!* Потому что нельзя доверять людям, чтобы они себя защищали!

b: Я пытаюсь защитить твою тупую задницу всю свою жизнь и сейчас ты просто с--

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

h: АХАХАХАХАХАХА

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: Ох, ВАУ, это самое большое *^ёбано^е* преуменьшение века!

`hong({ body:"yell_2" });`

h: Да, ты гниющая куча окровавленного ^дерьма^! Ты сильно ^проебал^ся!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Замечания, Капитан Очевидность?

[Но месть мне это не ответ!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Но в этот раз я *действительно* прав!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Я причинил тебе боль.](#act3_good_2a)


# act3_good_1_fail_revenge

b: Ты должен иметь более здоровые отношения со своими эмоциями, а не заглушать их чт--

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

b: Пожалуйста, опусти бутылку и давай--

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

h: Твой уровень энергии выглядит так ужасно, волк.

h: На твоём месте я бы тщательно подобрал свои следующие слова.

`bb({ eyes:"normal" });`

[Хорошо. Я перестану тебя защищать.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Я был прав с самого начала.](#act3_bad_2_right)

[Прости меня.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_2_jump

b: Ну что, вперёд, прыгай. Какое мне дело.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Тогда ладно. Пей до дна.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: НЕТ ПОДОЖДИ ЭТО БЫЛА ОБРАТНАЯ ПСИХОЛОГИЯ ТЫ ДОЛЖЕН БЫЛ СДЕЛАТЬ *ПРОТИВОПОЛОЖНОЕ* ТОМУ ЧТО Я СК--

(#act3_bad_3)

# act3_bad_2_right

`bb({ eyes:"angry" });`

b: Ты *подвергаешь* себя опасности. Твои, так называемые, друзья *используют* тебя. И *ты* используешь своих, так называемых, друзей.

`bb({ eyes:"sad" });`

b: Так что, пожалуйста, человек... почему ты мне не веришь?!

h: Потому что ты никогда не верил в *меня*.

(#act3_bad_3)

# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: У других сторожевых волков есть люди, которые действительно терпеливо тренируют их, *учатся* работать вместе,

b: Вместо того, чтобы ненавидеть сторожевых волков за их защиту! Так почему ты не можешь прос--

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

h: *"Единственное, чего нам нужно бояться, так это самого страха."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Не парься, будь счастлив!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Все мудрецы нашего времени согласны: отрицательные эмоции *плохие!*

`hong({ eyes:"less_angry" });`

h: Ах! Вот почему они называются *негативом!*

b: человек... пожалуйста...

`hong({ eyes:"normal" });`

h: Некоторое время назад я сказал: "Я просто хочу быть свободным от всей этой боли".

h: Я получил своё желание. Я больше не чувствую боли или страха, или тревоги...

h: Я больше ничего не чувствую.

`_.a3_ending = "jump";`

(#act3_end)

# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Я был так одержим убедиться, что больше ничего не причинит тебе вреда, что не осознавал, что *я* причинял боль.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: НИХРЕНА. СЕБЕ.

`hong({ body:"yell_1" });`

h: ^ПИЗДЕЦ^. Тебе действительно понадобилось так много времени, чтобы наконец понять это?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Ты мог бы спасти нас от стольких неприятностей, ты, большой пушистый, тупой ^придурок^. Почему ты не понял это раньше?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)

# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...ты *извиняешься.*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: Извиняешься за *что*?

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

[Прости, я не был хорошим защитником.](#act3_good_3_protector)

[Прости, я не уважал тебя.](#act3_good_3_respect)

[Прости меня.](#act3_good_4)

# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Прости, у меня отвратительный человек!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Прости, я не уважал тебя.](#act3_good_3_respect)

[Прости, я вредил тебе.](#act3_good_3_hurt)

# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: Я должен был предупреждать тебя о *реальной* опасности, но я лаял на машины и почтальона.

`bb({eyes:"sorry_up"});`

b: Лаял на тени. Слишком много лаял.

`bb({eyes:"sorry"});`

b: Имеет смысл только то, что ты захочешь мне врезать.

`bb({eyes:"sorry_down"});`

b: Прости меня.

(#act3_good_4)

# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: Я должен был быть *твоим* верным сторожевым псом, но я действовал так, как будто ты должен был подчиняться *мне*.

`bb({eyes:"sorry_up"});`

b: Есть разница между защитником и тюремным надзирателем, и я перегнул палку.

`bb({eyes:"sorry_down"});`

b: Прости меня.

(#act3_good_4)

# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Я был настолько одержим попытками защитить тебя от причинения вреда, что никогда не осознавал, что это *я* причинял тебе боль.

`bb({eyes:"sorry_up"});`

b: Я был плохой собакой.

`bb({eyes:"sorry_down"});`

b: Прости меня.

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

h: Да, в любом случае, это была глупая идея.

h: Я делал это только чтобы испортить тебя, и, ну, я тебя испортил.

h: Давай просто закончим этот раунд вничью, ладно?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Окей.

h: Окей.

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

r: О, *да ладно*. После всего что зверь сделал с тобой, ты просто *сдашься?*

r: В чём дело, малыш? Ты *испугался?*

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Да.

h2: Я напуган.

`publish('hong-next')`

h2: И это нормально!

`publish('hong-next')`

h2: Это нормально быть напуганным.

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

r: Он просто запер дверь?

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

b: не...

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

b: не не не

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
