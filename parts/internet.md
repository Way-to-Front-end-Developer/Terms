https://roadmap.sh/frontend

Internet - The Internet is a global network of computers connected to each other which communicate through a standardized set of protocols.
https://www.vox.com/2014/6/16/18076282/the-internet
https://developer.mozilla.org/en-US/docs/Glossary/Internet
https://developer.mozilla.org/en-US/docs/Glossary/IPv6

`DNS` - The Domain Name System (DNS) is the phonebook of the Internet. Humans access information online through domain names, like nytimes.com or espn.com.
Web browsers interact through Internet Protocol (IP) addresses. DNS translates domain names to IP addresses so browsers can load Internet resources.

`Domain Name` - A domain name is a unique, easy-to-remember address used to access websites, such as ‘google.com’, and ‘facebook.com’. Users can connect to websites using domain names thanks to the DNS system. A domain name is a string of text that maps to a numeric IP address

A uniform resource locator (URL), sometimes called a web address, contains the domain name of a site as well as other information, including the transfer protocol and the path. For example, in the URL ‘https://cloudflare.com/learning/’, ‘cloudflare.com’ is the domain name, while ‘https’ is the protocol and ‘/learning/’ is the path to a specific page on the website.

`Hoisting` - Web hosting is an online service that allows you to publish your website files onto the internet. So, anyone who has access to the internet has access to your website.

How does the internet work? https://developer.mozilla.org/en-US/docs/Learn/Common_questions/How_does_the_Internet_work

`HTTP` is the TCP/IP based application layer communication protocol which standardizes how the client and server communicate with each other.
It defines how the content is requested and transmitted across the internet.

An HTTP request is the way internet communications platforms such as web browsers ask for the information they need to load a website.
Each HTTP request made across the Internet carries with it a series of encoded data that carries different types of information.
A typical HTTP request contains:
HTTP version type, a URL, an HTTP method, HTTP request headers, Optional HTTP body.
https://webhamster.ru/mytetrashare/index/mtb339/1526829184r5da41sxmn  

### HTTP caching

https://developer.mozilla.org/en-US/docs/Web/HTTP/Caching  
https://devcenter.heroku.com/articles/increasing-application-performance-with-http-cache-headers  
https://www.w3.org/Protocols/rfc2616/rfc2616-sec13.html

The HTTP cache stores a response associated with a request and reuses the stored response for subsequent requests.   
HTTP caching occurs when the browser stores local copies of web resources for faster retrieval the next time the resource is required.  
`The goal of caching in HTTP`/1.1 is to eliminate the need to send requests in many cases, and to eliminate the need to send full responses in many other cases.   

Стратегии кэширования
`Cache only`  
Одна из самых простых стратегий. Как можно догадаться из названия, все запросы отправляются в кэш.  
Случаи использования - для получения доступа к статическим активам
 
`Network only`  
Клиент делает запрос, service worker перехватывает его и направляет в сеть.  
Случаи использования - при отсутствии аналогов offline, например с analytics pings и запросами non-GET.
 
`Cache falling back to network`  
Service worker делает запрос в кэш, и при отсутствии ответа запрос отправляется в сеть.  
Случаи использования - при разработке offline first приложения
 
`Network falling back to cache`  
Сначала service worker делает запрос к сети, и в случае успешного ответа он отправляется в кэш.  
Случаи использования - При разработке часто меняющихся страниц, например: страницы для записей или таблицы участников игры. Идеально подойдет для случая, когда в приоритете последние добавленные данные.
 
`Generic fallback (Резерв)`  
Когда оба запроса дают сбой как к кэшу, так и к сети, отображается общий резерв вместо черного экрана или ошибки.

Sources:
https://www.cloudflare.com/en-gb/learning/ddos/glossary/hypertext-transfer-protocol-http/
https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview

`Protocol`
https://developer.mozilla.org/en-US/docs/Glossary/Protocol

`Requests`
https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods

`Status`
https://developer.mozilla.org/en-US/docs/Web/HTTP/Status

### World Wide Web (Web, W3) 
https://developer.mozilla.org/en-US/docs/Glossary/World_Wide_Web  

`the Web` -  is an interconnected system of public webpages accessible through the Internet. 

Browsers and how they work?

A `web browser` is a software application that enables a user to access and display web pages or other online content through its graphical user interface.  
A Web browser or browser is a program that retrieves and displays pages from the Web, and lets users access further pages through hyperlinks. A browser is the most familiar type of user agent.

`Веб-страница` — документ или информационный ресурс Всемирной паутины, доступ к которому осуществляется с помощью веб-браузера.  

https://web.dev/howbrowserswork/

Веб-страница — документ или информационный ресурс Всемирной паутины, доступ к которому осуществляется с помощью веб-браузера.

How does a brouser render a web page?
https://webdevblog.ru/kak-brauzer-renderit-veb-stranicu/ https://blog.logrocket.com/how-browser-rendering-works-behind-scenes/

`URL`
https://www.techtarget.com/searchnetworking/definition/URL A URL (Uniform Resource Locator)
https://developer.mozilla.org/en-US/docs/Glossary/URL is a unique identifier used to locate a resource on the Internet. It is also referred to as a web address.
URLs consist of multiple parts -- including a protocol and domain name -- that tell a web browser how and where to retrieve a resource.

A host (also known as "network host") is a computer or other device that communicates with other hosts on a network.

`URI`
https://developer.mozilla.org/en-US/docs/Glossary/URI

`HTTPS` is a secure way to send data between a web server and a browser.
https://www.cloudflare.com/en-gb/learning/ssl/what-is-https/

### CORS
https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS

`Cross-Origin Resource Sharing` `CORS` — механизм, использующий дополнительные HTTP-заголовки, чтобы дать возможность агенту пользователя получать разрешения на доступ к выбранным ресурсам с сервера на источнике (домене), отличном от того, что сайт использует в данный момент.

Content Security Policy
Content Security Policy is a computer security standard introduced to prevent cross-site scripting, clickjacking and
other code injection attacks resulting from execution of malicious content in the trusted web page context. https://developer.mozilla.org/en-US/docs/Web/HTTP/CSP
https://web.dev/csp/

OWASP Security Risks
OWASP or Open Web Application Security Project is an online community that produces freely-available articles,
methodologies, documentation, tools, and technologies in the field of web application security.

### API  
 
An `API` (Application Programming Interface) is a set of features and rules that exist inside a software  
program (the application) enabling interaction with it through software - as opposed to a human user interface.  

In Web development, an API is generally a set of code features (e.g. methods, properties, events, and URLs) that  
a developer can use in their apps for interacting with components of a user's web browser, or other software/hardware  
on the user's computer, or third party websites and services.

### User agent  
https://developer.mozilla.org/en-US/docs/Glossary/User_agent

A `user agent` is a computer program representing a person, for example, a browser in a Web context.  
Besides a browser, a user agent could be a bot scraping webpages, a download manager, or another app accessing the Web.


### Hyperlink  
https://developer.mozilla.org/en-US/docs/Glossary/Hyperlink

`Hyperlinks` connect webpages or data items to one another.  
In HTML, <a> elements define hyperlinks from a spot on a webpage (like a text string or image)  
to another spot on some other webpage (or even on the same page).
 
`interseprots`

`идемпотентность` http https://developer.mozilla.org/ru/docs/Glossary/Idempotent
 
`Web API`
Для программирования на языке JavaScript понимать Web API не просто желательно, а обязательно. Сталкиваться с
интерфейсом прикладного программирования (Application Programming Interfaces) в JS вы будете повсеместно.

A`PI браузера` — это такие конструкции, которые встроены в браузер и предназначенные для облегчения разработки функциональности.
Сторонние API — конструкции, встроенные в сторонние платформы, такие как Twitter, Zendesk, Trello и т. д.
С их помощью функциональность этих платформ можно использовать в своих веб-приложениях. Если API в платформе предусмотрен,
к нему обязательно прилагается инструкция.

Broadly speaking, a worker is a script that runs on a thread separate to the browser’s main thread.
https://bitsofco.de/web-workers-vs-service-workers-vs-worklets/

`Service Worker API`
https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API

A `Service worker` is basically a script (JavaScript file) that runs in the background, separate from a web page and provides features that don't need a web page or user interaction. Some of the major features of service workers are Rich offline experiences(offline first web application development), periodic background syncs, push notifications, intercept and handle network requests and programmatically managing a cache of responses.

`Web Workers API`
https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Using_web_workers   
 
`Web Workers` это механизм, который позволяет скрипту выполняться в фоновом потоке, который отделен от основного потока веб-приложения. Преимущество заключается в том, что ресурсоёмкие вычисления могут выполняться в отдельном потоке, позволяя запустить основной (обычно пользовательский) поток без блокировки и замедления.  

`Examples`: рендеринг трёхмерных сцен, шифрование, предварительная загрузка данных, проверка правописания.
 
### Minification
 
`Minification` — процесс, направленный на уменьшение размера исходного кода путём удаления ненужных символов без изменения его функциональности.


`PWAs`
`Progressive web applications` (`PWAs`) are a type of mobile app delivered through the web, built using common web technologies including HTML, CSS and JavaScript. These PWAs are deployed to servers, accessible through URLs, and indexed by search engines.
 
### Long polling
`Long polling` – это самый простой способ поддерживать постоянное соединение с сервером, не используя при этом никаких специфических протоколов (типа WebSocket или Server Sent Events).
 
 
### WebSocket & Server Sent Events  
https://learn.javascript.ru/websocket

Протокол `WebSocket`, обеспечивает возможность обмена данными между браузером и сервером через постоянное соединение. Данные передаются по нему в обоих направлениях в виде «пакетов», без разрыва соединения и дополнительных HTTP-запросов.  
WebSocket особенно хорош для сервисов, которые нуждаются в постоянном обмене данными: онлайн игры, торговые площадки, работающие в реальном времени, и т.д.
`Ping-pong` фреймы - используется для проверки соединения; отправляется с сервера, браузер реагирует на них автоматически.

Спецификация `Server-Sent Events` описывает встроенный класс EventSource, который позволяет поддерживать соединение с сервером и получать от него события.
 
| WebSocket                            | EventSource                                     | 
| -------------------------------------| ------------------------------------------------| 
| Двунаправленность: и сервер, и клиент|Однонаправленность: данные посылает только сервер|
|могут обмениваться сообщениями        |                                                 | 
| Бинарные и текстовые данные          | Только текст                                    | 
| Протокол WebSocket                   | Протокол HTTP                                   | 
 
 
### Throttling & debouncing

`Throttling и debouncing` — это широко используемые техники для увеличения производительности кода, который выполняется повторно с некоторой периодичностью.

`Throttling` функции означает, что функция вызывается не более одного раза в указанный период времени (например, раз в 10 секунд). Другими словами ― Throttling предотвращает запуск функции, если она уже запускалась недавно. Throttling также обеспечивает регулярность выполнение функции с заданной периодичностью.
```
 function throttle(cb, delay = 250) {
  let shouldWait = false
 
  return (...args) => {
    if (shouldWait) return
 
    cb(...args)
    shouldWait = true
    setTimeout(() => {
      shouldWait = false
    }, delay)
  }
}
```
 
`Debouncing` функции означает, что все вызовы будут игнорироваться до тех пор, пока они не прекратятся на определённый период времени. Только после этого функция будет вызвана.
 
```
function debounce(cb, delay = 250) {
  let timeout
 
  return (...args) => {
    clearTimeout(timeout)
    timeout = setTimeout(() => {
      cb(...args)
    }, delay)
  }
}
```

