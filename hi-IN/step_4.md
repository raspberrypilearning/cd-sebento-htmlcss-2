## अपने पृष्ठ का आयोजन

अब तक आपने **कन्टेन्ट** देखने और पढ़ने में आसान बनाने के लिए **शीर्षकों**और **पैराग्राफ** का उपयोग किया है। आइए एक साथ चीजों को समूहीकृत करके इसे और भी व्यवस्थित करें।

--- collapse ---
---
title: कन्टेन्ट क्या है?
---

**कन्टेन्ट** आपके वेब पृष्ठ पर सब कुछ है, जैसे की टेक्स्ट और चित्र।

--- /collapse ---

+ `birds.html` फ़ाइल में जाएं (या यदि आप उदाहरण प्रोजेक्ट का उपयोग नहीं कर रहे हैं तो अपने स्वयं के पृष्ठों में से एकमें जाएं) और, शीर्ष के पास, उदघाटन टैग `<main>` के **नीचे**, नई लाइन पर निम्नलिखित टाइप करें:

```html
  <main>
    <article>
```

+ यदि आपका एडिटर अपने आप, आपके लिए एक समापन `</article>` टैग जोड़ता है तो, उसे मिटाएं।

+ फ़ाइल के निचले भाग में, समापन `</main>` टैग के ** ऊपर **, एक नई पंक्ति जोड़ें और ` article ` एलीमेंट बंद करें:

```html
    </article>
  </main>
```

आपका `main` एलीमेंट अब कुछ ऐसा दिखना चाहिए (आपके `article` टैग के बीच भिन्न सामग्री हो सकती है):

```html
  <main>
    <article>
      <h1>Birds of conservation concern in Ireland</h1>
      <p>
       There are a number of birds in Ireland whose numbers are in decline.
       Some of those with a high priority for conservation are:
      </p>  

      <h2>Barn Owl</h2>
      <p>The barn owl is the most common owl and is found in most parts of the world. 
      It has seen a huge decline in Ireland and Europe in recent years.</p>
      <img src="barn-owl-landing.jpg" alt="Barn owl landing on a branch" height="200px" />
      <h2>Curlew</h2>
      <p>The curlew is recognisable by its long curved bill.
      </p>
      <img src="curlew.jpg" width="200px" />
      <p>Curlews use their long bills to search for worms in mud or very soft ground.
      </p>
      <img src="curlew2.jpg" width="200px" />
    </article>
  </main>
```

+ अब अपने `article` में कन्टेन्ट को देखें और इसे खंडों में तोड़ने का प्रयास करें। टैग की इस नई जोड़ी को प्रत्येक बिट के आसपास रखें: `<section> </section>` यहाँ एक उदाहरण है कि यह कैसा दिख सकता है:

```html
  <article>
    <h1>My favourite places to see in Ireland</h1>
    <section>
      <h2>Barn Owl</h2>
      <p>The barn owl is the most common owl and is found in most parts of the world. 
      It has seen a huge decline in Ireland and Europe in recent years.</p>
      <img src="barn-owl-landing.jpg" alt="Barn owl landing on a branch" height="200px" />
    </section>
    <section>
      <h2>Curlew</h2>
      <p>The curlew is recognisable by its long curved bill.
      </p>
      <img src="curlew.jpg" width="200px" />
      <p>Curlews use their long bills to search for worms in mud or very soft ground.
      </p>
      <img src="curlew2.jpg" width="200px" />
    </section>
  </article>
```

--- collapse ---
---
title: नए टैग क्या हैं?
---

इन नए एलीमेंट्स को ** कंटेनरों** के रूप में सोचें। उनका उपयोग चीजों को एक साथ समूहित करने के लिए किया जाता है। यह आपके घर में बक्से और अलमारियों में चीजों को व्यवस्थित करने जैसा है!

यह आपकी वेबसाइट को स्क्रीन रीडर्स के लिए अनुकूल बनाता है, आपको वेबसाइट के लेआउट पर अधिक नियंत्रण देता है, और, जैसा कि आप देखेंगे, यह आपको स्टाइल के साथ वास्तव में रचनात्मक बनने की अनुमति देता है।

टैग के बीच में कुछ भी लिखा जा सकता है। आमतौर पर यह एक से अधिक एलीमेंट होगा, लेकिन यह होना जरूरी नहीं है। यह किसी भी तरह का HTML एलीमेंट हो सकता है। आप जो कर रहे हैं वह ब्राउज़र को बता रहा है कि इन टैगों के बीच सब कुछ एक साथ है।

### Article

` article ` एलीमेंट सामग्री के एक पूरे टुकड़े के लिए एक कंटेनर है, इस मामले में आयरलैंड में आकर्षण के बारे में जानकारी का एक सेट है। यदि आपके पास अलग-अलग कन्टेन्ट है जो संबंधित नहीं हैं, तो पूरे कन्टेन्ट के चारों ओर टैग का एक सेट लगाने के बजाय, आपको प्रत्येक को अपने ` article ` एलीमेंट में डालना चाहिए ।

### Section

`section` एलीमेंट आपको संबंधित कन्टेन्ट को छोटे टुकड़ों में विभाजित करने और प्रत्येक टुकड़े को अपने कंटेनर में रखने की सुविधा देता है।

### अन्य भी मौजूद हैं!

HTML में केवल ये कंटेनर एलीमेंट नहीं हैं। यदि आपने कभी मेन्यू बनाया है और फिर उसे `<nav> </nav>` टैग के बीच में रखा है, यह एक और प्रकार का कंटेनर है। वैसे ही `<main> </main>` और `<header> </header>` हैं- क्या आप किसी और के बारे में सोच सकते हैं?

--- /collapse ---

--- challenge ---

हो सकता है कि आपका वेब पृष्ठ अभी अलग न दिखे, लेकिन एक बार कंटेंट कंटेनर टैग में व्यवस्थित हो जाने के बाद, आप इसमें CSS के साथ कुछ अच्छी चीजें करने में सक्षम होंगे। याद रखें, HTML नियंत्रित करता है कि आपकी वेबसाइट कैसे व्यवस्थित है, और CSS यह कैसी दिखती है।

## चुनौती: अपनी वेबसाइट व्यवस्थित करें

+ इस तरह से `article` और `section` कंटेनर का उपयोग करके अपनी वेबसाइट के सभी कन्टेन्ट को व्यवस्थित करने पर ध्यान दें।

--- hints ---

--- hint ---

उदाहरण प्रोजैक्ट के संरक्षण पृष्ठ को देखें। आप देखेंगे कि हमने `conservation.html` फ़ाइल में एक `article ` के साथ और कई`section` टैग जोड़े हैं:

```html
  <main>
        <article>

        <h1>Conservation efforts</h1>
        <p>
         Various kinds of work are carried out in Ireland in order to protect bird species.
        </p>  

        <section>
          <h2>Research and monitoring</h2>
          <p>
            An essential part of bird conservation is monitoring and recording 
            information about the species such as their numbers, breeding habits, etc. 

          </p>
          <p>
            Scientific research may be carried out to determine whether a species is 
            in decline and how to address the problem.
          </p>
        </section>

        <section>
          <h2>Habitat protection</h2>
          <p>
            The destruction of habitat is a serious threat to many birds and 
            therefore protecting habitats is crucial to protecting the species.
          </p>

          <p>One example of this is the preservation of wetlands in Ireland.</p>
        </section>

        <section>
          <h2>Control invasive plants and animals</h2>
          <p>
            Mink and rats are a predator that threaten many bird species, 
            for example by eating their eggs.
          </p>
          <p>
            Rhododendron is an example of an invasive plant which can very quickly
            take over large areas of countryside, disrupting the biodiversity.
          </p>
        </section>
        </article>   
  </main>
```

--- /hint ---

--- /hints ---

अगले कार्ड पर, आप प्रत्येक पृष्ठ के लिए एक अलग थीम डिज़ाइन करेंगे जो लेखों और अनुभागों में व्यवस्थित होगी!

--- /challenge ---
