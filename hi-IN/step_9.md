## एनीमेशन

क्या आप जानते हैं कि आप चीजों को चारों ओर घूमाने के लिए CSS का उपयोग कर सकते हैं? आप इस कार्ड से यही सीखेंगे!

+ आरंभ करने से पहले, सुनिश्चित करें कि आपके पास `id` के साथ आपकी वेबसाइट पर एक तस्वीर है और उसके लिए एक CSS खंड जो की `width` को `100px` निर्धारित करता है। मैं पहले वाली खलिहान के उल्लू की तस्वीर का इस्तेमाल करने जा रहा हूं, और मेरा CSS खंड इस तरह दिखता है:

```css
    #owly {
        border-radius: 100%;
        width: 100px;
    }
```

+ अपनी CSS फाइल के नीचे जाएँ और निम्न कोड जोड़ें:

```css
    @keyframes myFirstAnimation {
        from {
            width: 100px;
        }
        to {
            width: 300px;
        }
    }
```

यह कोड `myFirstAnimation` नामक एक एनीमेशन बनाता है जिसको आप अपनी वेबसाइट पर किसी भी एलीमेंट से जोड़ सकते हैं। आपको क्या लगता है यह क्या करेगा?

+ चित्र के लिए अपने CSS नियम खोजें और निम्नलिखित तीन प्रॉपर्टीज जोड़ें:

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ अब देखें कि आपके वेब पृष्ठ पर क्या होता है! `animation-iteration-count` के लिए अलग-अलग मान आज़माएं और देखें की यह क्या करता है।

+ चलिये एक और एनीमेशन का इस्तेमाल करते हैं! निम्नलिखित कोड को अपनी CSS फाइल के आखिर में जोड़ें:

```css
    @keyframes rainbowGlow {
        0% {
            color: #FFD700;
        }
        50% {
            color: #663399;
        }
        100% {
            color: #FFD700;
        }
    }
```

+ अब पहले से लिखे ` #myCoolText ` के CSS नियमों को ढूँढें और एनीमेशन कोड जोड़ें:

```css
    #myCoolText {        
        color: #003366;
        border: 2px ridge #ccffff;
        padding: 15px;
        text-align: center;
        animation-name: rainbowGlow;
        animation-duration: 1.5s;
        animation-iteration-count: 1;
    }
```

जब आप `से` और `तक` के बजाय **प्रतिशत मान** का उपयोग करते हैं, तो आप दो मानों के बीच में और साथ ही शुरू और अंत वाले मान सेट करने में सक्षम होते हैं। आप ` 0 ` से अलग-अलग प्रतिशत मानों का उपयोग करते हुए ` 100 ` तक जितना चाहें उतना मूल्य सेट कर सकते हैं।

+ `animation-iteration-count` के मान को बदलकर `infinite` करें। देखें कि आपके परीक्षण करने से पहले क्या आप अनुमान लगा सकते हैं कि क्या होगा!

+ अपने एनीमेशन को गति देने या धीमा करने के लिए `animation-duration` के लिए अलग-अलग मान आज़माएं।

+ एक अंतिम चाल! इस एनीमेशन कोड को जोड़ें:

```css
    @keyframes slide {
        0% {
            background-position-x: 0;
        }
        100% {
            background-position-x: 600vw;
        }
    }
```

+ अब ` #frontPage ` के CSS नियम जो आपने पहले लिखे थे ढूंढें और उन्हें इसमें बदलें:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

ऊपर के पूर्ण कोड को समझने की चिंता न करें... बस आराम से बैठें और आनंद लें!!

एनीमेशन के साथ आप और अधिक चीज़ें कर सकते हैं, उनके बारे में जानने के लिए, [इस वेब पृष्ठ](http://dojo.soy/se-css-animation){:target="_blank"} पर जाएं। मजे करें!

अगले कार्ड पर आप सीखेंगे कि जब आप चीजों पर माउस कर्सर घुमाते हैं तो रोचक चीजें कैसे होती हैं!
