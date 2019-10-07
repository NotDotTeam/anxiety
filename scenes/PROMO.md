# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[ИГРАТЬ!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Прежде чем мы начнём, как бы *тебе* хотелось читать?

`publish("show_options_bottom")`

# intro-start-2

n3: А сейчас, начнём нашу историю..

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: ЭТО ЧЕЛОВЕК

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: А ЭТО ТРЕВОГА ЧЕЛОВЕКА

n: _ТЫ_ ЭТА ТРЕВОГА

(#act1_normal)

# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Не. Нет, не-а, не слушаю. Проверю свой телефон.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: ТВОЯ РАБОТА ЗАЩИЩАТЬ ТВОЕГО ЧЕЛОВЕКА ОТ *ОПАСНОСТИ*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Ты проскроливаешь свою жизнь в Twitter! Опять!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Да, я удивляюсь, почему я не просто сижу и слушаю свои мысли почаще.

`hong({eyes:"neutral"});`

n: БЫСТРЕЕ, ПРЕДУПРЕДИ ЕГО ОБ *ОПАСНОСТИ!*

```
bb({eyes:"look"});
```

[О нет, взгляни на эту ужасную историю в новостях!](#act1d_news)

[О нет, эти твиты в действительности о *нас?*](#act1d_subtweet)

[Эй, GIF-ка о котике лакающий молочко](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h:  Хех, да, это довольно мило, Я--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: КОШКИ НЕ ПЕРЕВАРИВАЮТ МОЛОКО, И МЫ УЖАСНЫЕ ЛЮДИ НАСЛАЖДАЮЩИЕСЯ НАСИЛИЕМ НАД ЖИВОТНЫМИ

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



