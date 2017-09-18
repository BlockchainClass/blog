+++
title = "Obelisk: Алгоритм консенсуса проекта Skycoin"
tags = [
    "Statement",
]
date = "2017-09-08"
categories = [
    "Statement",
]
+++

*Алгоритм консенсуса проекта Skycoin называется "Obelisk" и детально описан в
[whitepapers](https://www.skycoin.net/whitepapers)*

Блокчейн Skycoin использует новый тип алгоритма консенсуса, называемый
"Obelisk", который заменяет и Proof of Work (“PoW”), и Proof of Stake
(“PoS”).

Цель разработчиков Skycoin - исправить основные недостатки в обеспечении 
безопасности и «централизующие тенденции», свойственные блокчейнам, консенсус 
которых основан на алгоритмах PoW или PoS, а создание монет основано на
майнинге. Поэтому Skycoin пытается создать криптовалюту, которая больше 
соответствует оригинальному видению Satoshi полностью децентрализованной 
цифровой валютной системы.

При этом технология Skycoin создает блокчейн без необходимости майнинга,
с фиксированными объемами крипто-токенов, 10-секундными транзакциями 
и отличной системой безопасности. 
Если в системе искажена связь между созданием токенов и контролем над сетью,
крипто-токены теряют политическую функцию и становятся скорее формой цифрового 
имущества в прямом смысле слова.

## Proof of Work и система биткойна

Фундаментальный просчет при раннем программировании биткойна заключается в том, 
что процесс майнинга является основой экономической структуры стимулирования, 
которая должна содействовать децентрализации. Фактически же связь между консенсусом 
и вычислительной мощностью хеширования стимулирует приобретение все увеличивающихся
мощностей и приводит к риску установления частного контроля над коненсусом сети.

Например, сеть Биткойн де-факто контролируется тремя коммерческими майнинговыми пулами,
которые смогли сосредоточить значительную часть мощностей хеширование на своих серверах.
Эти пулы начали действовать как картель, разделяя мощности хеширования между собой 
по договоренности. Связь между майнингом и контролем сети была указана Satoshi в качестве
основной не-криптографической угрозы стабильности сети. Это позволяет игрокам, 
сосредоточившим в своих руках достаточную вычислительную мощность и достигшим
преобладания в хеш-рейте, при атаке 51% или фальсифицировать, или обращать 
транзакции в сети. Утверждают, что эта уязвимость стала менее актуальной в ситуации,
когда хеш-мощность сосредоточена в руках лиц, вложивших большие деньги в сеть
биткойн и их выживание зависит от высокой стоимости биткойна. Однако это не меняет
факта, что способность влиять на сеть находится в чьих-то руках и искажена
сама суть криптовалюты, основанной на децентрализованном распределенном реестре.
  
Таким образом, алгоритм PoW сети биткойн имеет проблемы в области безопасности
и монополизации через установление власти над сетью лицами, способными
мобилизовать достаточные экономические ресурсы для контроля процесса майнинга.

Это также означает, что работа сети как экономически, так и экологически 
неэффективна. Продолжается все возрастающий ввод мощностей для майнинга,
потребляется большое количество электроэнергии, ежемесячно уже на десятки 
миллионов. Эти затраты могут быть компенсированы только экспоненциально 
растущим притоком новых пользователей с вливанием дополнительного капитала.

Только очень небольшое количество устоявшихся монет, таких как биткойн и эфириум, 
способны привлекать достаточное количество пользователей для достижения подобного 
непрерывного потока. Большинство же монет на основе PoW / PoS обречено, 
так как при недостатке притока капитала стоимость майнинга PoW / PoS будет 
вынуждено оплачиваться по более низкой ставке, цена монет будет приближаться
к цене майнинга до тех пор, пока монета не будет брошена.
  
В настоящее время экономика биткойна основана на новых пользователях, 
вкладывающих свои деньги, затем деньги бросают в яму майнинга и сжигают в 
ритуале жертвоприношения на алтаре стоимости электричества. Если средний 
пользователь должен будет платить гонорары майнерам, покрывая их затраты 
на электроэнергию напрямую в качестве транзакционных сборов, вместо того
чтобы быть ограбленным ими через инфляцию путем создания новых биткойнов, 
то каждая биткойн транзакция будет стоить более 50 долларов США. Это дороже, 
чем международный банковский перевод.
 
## Тенденция централизации Proof of Stake

Несмотря на то, что алгоритмы Proof of Stake устраняют проблему устойчивости 
против атаки 51%, они потенциально даже более уязвимы к централизации, 
чем сети PoW. 
В PoS размер депозитов криптовалюты участников сети определяет
их полномочия и право голоса при внесении технических изменений в сеть. 
Участники могут получать эквивалентную их доле часть наград вне зависимости
от вычислительной мощности.

Этот принцип значительно увеличивает экономические барьеры для атаки 51%, 
потому что финансовые затраты на приобретение большинства токенов в
сети на открытом рынке скорее всего превысят потенциальный выигрыш. Если
злоумышленник окажется в роли основного участника сети, он больше всех 
и пострадает от атаки на стабильность сети или на внешнюю цену криптовалюты.

Тем не менее, несмотря на увеличение барьеров против вызванных людьми нападений, 
PoS создает централизующий импульс, причем столь же сильный, если не сильнее, 
чем в случай PoW. Джозеф Янг подводит итог в своем сравнении двух систем на
[coinfox.info](http://www.coinfox.info/): «Система, в которой основная
заинтересованная сторона объединяет расширенный контроль и полномочия как 
по техническим, так и по экономическим аспектам сети, получает серьезную 
проблему монополизации». В то время как в PoW-голосование по внедрению
технических изменений в сеть "поделено среди майнеров, разработчиков и 
других важных членов сообщества", в PoS системе "основные заинтересованные 
стороны имеют техническую возможность вносить какие-либо изменения в сеть
без учета мнения сообщества, бизнеса, майнеров и разработчиков. Эта 
централизация полномочий голосования и, по сути, контроль сети уничтожает
основу криптовалюты на базе распределенного реестра, поскольку противоречит
принципу распределения всех элементов в сети для устранения центрального органа».
 
## Obelisk: алгоритм распределенного консенсуса

Чтобы решить проблему централизации, Skycoin выходит за рамки PoW / PoS.
Он использует распределенный алгоритм консенсуса, называемый Obelisk, который
определяет влияние узла на сеть в соответствии с подходом «web of trust». 
По сути, каждый узел имеет список других доверенных узлов, на которые он 
подписывается, и плотность сети подписчиков узла определяет его влияние на сеть.
Каждый узел ведет персональный блокчейн, который действует как «общедоступный
канал", на котором видны и публично записаны все действия узла. Поскольку 
все консенсусные решения и общение происходят через персональный блокчейн 
каждого узла, сообщество может очень легко проверить узлы на предмет обмана
или сговора. Механизм прининятия решений в сети и степень влияния узлов на эти 
решения общедоступны и прозрачны.

Публичная запись действий каждого узла в приватном блокчейне позволяет сети
реагировать на отступничество путем разрыва соединений с менее надежными или
вредоносными узлами, сокращая сеть до меньшего и более плотного ядра
доверенных узлов. Следовательно, если сообщество не доверяет некоторым узлам
или чувствует, что мощность внутри сети слишком сконцентрирована
(или недостаточно сконцентрирована), оно может коллективно изменить баланс 
сил в сети путем коллективного изменения доверительных отношений с узлами. 
Подотчетность узлов сообществу и внешние аудиты, а также прозрачность 
консенсуса усиливают коллегиальность принятия решений и, таким образом, 
вводят очень демократичные и децентрализованные элементы в сеть.
  
Такой подход обеспечивает системе цифровой валюты значительное уменьшение
времени транзакций, отсутствие майнинга и отличную безопасность.

Читайте [Skycoin whitepapers](https://www.skycoin.net/whitepapers), 
чтоб больше узнать про Obelisk.