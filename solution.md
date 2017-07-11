```
function decode(toDecode) {
    var decodeBetterThanAES = '';
    toDecode = toDecode.split().reverse().join();
    for (var i = 0; i < toDecode.length; i++) {
        var transformed = toDecode[i].charCodeAt() - key[i].charCodeAt() + i;
        decodeBetterThanAES += String.fromCharCode(transformed);
    }
    return decodeBetterThanAES;
}
window.decode = decode;
```

Key: `GrevyoabVasapByRujocsetnatVaseannEajOitGehakOlWercyutDeomRagDyd!`

Message: `Gratulacje :) Spotkanie odbywa się dnia 10.07.2017 w godzinach 15:00 - 19:30 w sali demowej. Aby zapisać się na hackathon napisz maila na adres jakub.lechocki+hackathonBezpCRM@rst.com.pl`

Encrypted message: `U2FsdGVkX1+258ryzRLHMU6yGs7MebzJX4Icng2Xlgz/iWeN314rKNGZlnZh1K39cFg+l7eTlSG716MampLLMIGMX6T/37GyP4oWglgEbCsAfwRglnK0uCmLk7EjxItaQeg/QyO9buvuVL2crMfuT/O/30pqYLiBW+ZPjQBJ0DB+ZSm8rywYJP+jsMMLgragOzogXZ+nAjtXyfbDmwN16a7rSDIRGnVDaIXr7gwY/MQWxl657gunmTNuC/SjWPMf0TIzlVxEsNA68/tGPD1fRg==`
