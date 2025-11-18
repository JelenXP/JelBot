# Economy Bot – Dokumentace

Verze: beta 1.0.0

# Popis:
Economy Bot je Discord bot pro správu herní měny Jelcoins a kreditů na serveru. Umožňuje uživatelům nakupovat, prodávat, sbírat Jelcoiny a nakupovat role ve shopu. Administrátorům poskytuje nástroje pro správu uživatelů a nastavení shopu.

# Uživatelské příkazy
j!buyjel <amount>

Popis: Koupí zadané množství Jelcoinů za aktuální cenu v kreditech.

Funkce:

Vypočítá celkovou cenu včetně poplatku 4%.

Zobrazí potvrzovací embed s tlačítky „Přijmout / Odmítnout“.

Při potvrzení:

Odečte kredity uživatele.

Přidá Jelcoiny.

Přičte poplatek k celkovým poplatkům.

Aktualizuje cenu Jelcoinu.

Limity: Max. 1 000 000 000 Jelcoinů najednou.

Chyby: Nesprávný formát příkazu nebo nedostatek kreditů zobrazí embed s informací a nápovědou.

j!selljel <amount>

Popis: Prodá zadané množství Jelcoinů za aktuální cenu v kreditech.

Funkce:

Odečte Jelcoiny uživatele.

Přičte kredity minus poplatek 6%.

Aktualizuje cenu Jelcoinu.

Limity: Max. 1 000 000 000 Jelcoinů najednou.

Chyby: Pokud uživatel nemá dostatek Jelcoinů, zobrazí se embed s chybou.

j!stats

Popis: Zobrazí uživatelské a globální statistiky ekonomiky.

Funkce:

Zobrazuje počet kreditů a Jelcoinů uživatele.

Pořadí uživatele v serveru podle množství kreditů a Jelcoinů.

Celkové množství Jelcoinů a kreditů na serveru.

Aktuální cenu Jelcoinu.

j!mine

Popis: Umožňuje uživateli „mine“ Jelcoiny jednou za 24 hodin.

Funkce:

Náhodně generuje 0,5–10 Jelcoinů.

15% šance na bonus 0,5–3 Jelcoinů.

Přidává Jelcoiny uživateli.

Aktualizuje statistiky a cenu Jelcoinu.

Omezení: Jednou za 24 hodin na uživatele. Embed zobrazuje hlavní výtěžek, bonus a celkový výtěžek.

j!shop

Popis: Zobrazí shop serveru s dostupnými rolemi.

Funkce:

Načte role a jejich ceny z databáze.

Umožní interaktivní nákup přes tlačítka.

Potvrzení nákupu přidá roli uživateli a odečte kredity/jelcoiny podle ceny.

Poznámka: Pokud uživatel nemá dostatečné prostředky, zobrazí se chybový embed.

j!poplatky

Popis: Zobrazí celkové nasbírané poplatky z nákupů Jelcoinů.

Funkce: Vypíše celkovou částku nasbíranou do fee účtu.

j!verze

Popis: Zobrazí verzi bota.

Funkce: Embed zobrazující aktuální verzi bota (beta 1.0.0).

Administrátorské příkazy
j!add <@user> <amount> <credits/jelcoins>

Popis: Přidá zadané množství kreditů nebo Jelcoinů uživateli.

Funkce:

Podporuje typ credits nebo jelcoins.

Změní uživatelský zůstatek a zobrazí potvrzení embed.

Omezení: Pouze pro administrátory.

j!reset <@user>

Popis: Resetuje uživatelský účet nebo vybranou měnu.

Funkce:

Nabízí dropdown menu s možnostmi: Všechno / Credits / Jelcoins.

Po výběru zobrazí tlačítka pro potvrzení nebo zrušení.

Reset aktualizuje databázi a odebere hodnoty podle výběru.

Omezení: Pouze pro administrátory.

j!shopset <@role> <amount> <credits/jelcoins>

Popis: Přidá roli do shopu s určenou cenou a měnou.

Funkce: Vloží záznam do databáze shopu a zobrazí potvrzení embed.

j!shopdel <id>

Popis: Odstraní položku ze shopu podle ID.

Funkce: Vymaže záznam z databáze a potvrdí akci embedem.

Další vlastnosti

Dynamická cena Jelcoinů: Cena se zvyšuje při nákupu a snižuje při prodeji.

Poplatky: Fee se přidává při každém nákupu/prodeji Jelcoinů.

Chyby a validace:

Embed zprávy informují o nesprávném formátu příkazů.

Omezení podle rolí (administrátor) a cooldowny.

Interaktivní potvrzení: U nákupů a resetů se používají tlačítka a dropdown menu pro potvrzení. JelBot – Dokumentace

Verze: beta 1.0.0

Popis:
Economy Bot je Discord bot pro správu herní měny Jelcoins a kreditů na serveru. Umožňuje uživatelům nakupovat, prodávat, sbírat Jelcoiny a nakupovat role ve shopu. Administrátorům poskytuje nástroje pro správu uživatelů a nastavení shopu.

Uživatelské příkazy
j!buyjel <amount>

Popis: Koupí zadané množství Jelcoinů za aktuální cenu v kreditech.

Funkce:

Vypočítá celkovou cenu včetně poplatku 4%.

Zobrazí potvrzovací embed s tlačítky „Přijmout / Odmítnout“.

Při potvrzení:

Odečte kredity uživatele.

Přidá Jelcoiny.

Přičte poplatek k celkovým poplatkům.

Aktualizuje cenu Jelcoinu.

Limity: Max. 1 000 000 000 Jelcoinů najednou.

Chyby: Nesprávný formát příkazu nebo nedostatek kreditů zobrazí embed s informací a nápovědou.

j!selljel <amount>

Popis: Prodá zadané množství Jelcoinů za aktuální cenu v kreditech.

Funkce:

Odečte Jelcoiny uživatele.

Přičte kredity minus poplatek 6%.

Aktualizuje cenu Jelcoinu.

Limity: Max. 1 000 000 000 Jelcoinů najednou.

Chyby: Pokud uživatel nemá dostatek Jelcoinů, zobrazí se embed s chybou.

j!stats

Popis: Zobrazí uživatelské a globální statistiky ekonomiky.

Funkce:

Zobrazuje počet kreditů a Jelcoinů uživatele.

Pořadí uživatele v serveru podle množství kreditů a Jelcoinů.

Celkové množství Jelcoinů a kreditů na serveru.

Aktuální cenu Jelcoinu.

j!mine

Popis: Umožňuje uživateli „mine“ Jelcoiny jednou za 24 hodin.

Funkce:

Náhodně generuje 0,5–10 Jelcoinů.

15% šance na bonus 0,5–3 Jelcoinů.

Přidává Jelcoiny uživateli.

Aktualizuje statistiky a cenu Jelcoinu.

Omezení: Jednou za 24 hodin na uživatele. Embed zobrazuje hlavní výtěžek, bonus a celkový výtěžek.

j!shop

Popis: Zobrazí shop serveru s dostupnými rolemi.

Funkce:

Načte role a jejich ceny z databáze.

Umožní interaktivní nákup přes tlačítka.

Potvrzení nákupu přidá roli uživateli a odečte kredity/jelcoiny podle ceny.

Poznámka: Pokud uživatel nemá dostatečné prostředky, zobrazí se chybový embed.

j!poplatky

Popis: Zobrazí celkové nasbírané poplatky z nákupů Jelcoinů.

Funkce: Vypíše celkovou částku nasbíranou do fee účtu.

j!verze

Popis: Zobrazí verzi bota.

Funkce: Embed zobrazující aktuální verzi bota (beta 1.0.0).

Administrátorské příkazy
j!add <@user> <amount> <credits/jelcoins>

Popis: Přidá zadané množství kreditů nebo Jelcoinů uživateli.

Funkce:

Podporuje typ credits nebo jelcoins.

Změní uživatelský zůstatek a zobrazí potvrzení embed.

Omezení: Pouze pro administrátory.

j!reset <@user>

Popis: Resetuje uživatelský účet nebo vybranou měnu.

Funkce:

Nabízí dropdown menu s možnostmi: Všechno / Credits / Jelcoins.

Po výběru zobrazí tlačítka pro potvrzení nebo zrušení.

Reset aktualizuje databázi a odebere hodnoty podle výběru.

Omezení: Pouze pro administrátory.

j!shopset <@role> <amount> <credits/jelcoins>

Popis: Přidá roli do shopu s určenou cenou a měnou.

Funkce: Vloží záznam do databáze shopu a zobrazí potvrzení embed.

j!shopdel <id>

Popis: Odstraní položku ze shopu podle ID.

Funkce: Vymaže záznam z databáze a potvrdí akci embedem.

Další vlastnosti

Dynamická cena Jelcoinů: Cena se zvyšuje při nákupu a snižuje při prodeji.

Poplatky: Fee se přidává při každém nákupu/prodeji Jelcoinů.

Chyby a validace:

Embed zprávy informují o nesprávném formátu příkazů.

Omezení podle rolí (administrátor) a cooldowny.

Interaktivní potvrzení: U nákupů a resetů se používají tlačítka a dropdown menu pro potvrzení.
