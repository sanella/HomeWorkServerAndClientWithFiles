# HomeWorkServerAndClientWithFiles

Napraviti server koji provjerava pasvord od usera, ukoliko je tacan salje  mu jedan citat/jednu liniju iz file-a koji smo ranije napravili na nasem Desktopu,
te zapisuje u prazni file na nasem Desktopu.
Ukoliko pass nije tacan onda mu saljemo poruku da je netacan unos i njegovu IP adresu zapisujemo, datum i vrijeme pokusaja pristupa serveru.


Random quote generator (Kostur).
1. Generator. (server - server socket)
2. Client. (socket)
3. File Reader. (server)
4. File struktura (linija, quote) (server)
                  (linija, quote)
5. Spasavati quote-ove u fajl koji ce imati format: [TIMESTAMP]quote.

Server ima final pass.
Client salje serveru pass 
if(pass true)
vrati random quote.
else
 ispisi pass nije tacan.
4. 
6. Logovati pogresan pass kada pokusaj nije tacan i u kom vremenu - format [TIMESTAMP] pass.(server)

(Razrada)
-----------------------------
1. Naziv: RQG
2. Java
3. Package: ba.bitcamp.rqg.server
             - Generator.java
           ba.bitcamp.rqg.client
             - User.java
4. File location: Desktop (system agnostic)
5. Port: 1717
6. Repo: BITCampRandomQuoteGenerator
7. 15 guotes
8. [yyyy-mm-dd h:i:s]
9. [D] - quote
10. Server IP [input] ()
11. pass [input] Client (Password handling (pass se proslijedi na klijentu))
12. pass final static (na serveru je pass zakucan)
13. quotes.txt (fajl iz kojeg citamo quotes)
14. auth_log.txt (dio na serveru koji loguje pogresne pokusaje) - [D] - pass - IP (java socket get IP - procitati)  
15. recieved_quotes.txt Client 



Citati:
1. “So many books, so little time.”  ? Frank Zappa.
2. “No one can make you feel inferior without your consent.” ? Eleanor Roosevelt, This is My Story
3. “If you tell the truth, you don't have to remember anything.” ? Mark Twain
4. “If you tell the truth, you don't have to remember anything.” ? Mark Twain
5. “Live as if you were to die tomorrow. Learn as if you were to live forever.”? Mahatma Gandhi
6. “Without music, life would be a mistake.” 
7. “We accept the love we think we deserve.” ? Stephen Chbosky
8. “Good friends, good books, and a sleepy conscience: this is the ideal life.” ? Mark Twain
9. “If you don't stand for something you will fall for anything.” ? Gordon A. Eadie
10. “I have not failed. I've just found 10,000 ways that won't work.” ? Thomas A. Edison
11. “That which does not kill us makes us stronger.” ? Friedrich Nietzsche
12. “Choose a job you love, and you will never have to work a day in your life.” ? Confucius
13. “But better to get hurt by the truth than comforted with a lie.” ? Khaled Hosseini
14.“A person's a person, no matter how small.” ? Dr. Seuss
15. “A day without laughter is a day wasted.” ? Nicolas Chamfort
