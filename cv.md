# Dmitry Dudin
### Frontend Developer

---

### Contact information:

**Phone:** +7 (963)4665120<br>
**E-mail:** dmitrodonskoy@yandex.ru<br>
**Telegram:** @THANATASS<br>
[HeadHunter](https://hh.ru/resume/fab1aeb9ff08bb51ed0039ed1f496379313442)<br>

---

### Briefly About Myself:



---

### Skills and Proficiency:

- HTML5, CSS3, SCSS, CSS-modules
- JavaScript/TypeScript, C#
- React, Node.js, Next.js, Git

---

### Code example:

**Algorithmic problem:**
*Lapland is a one-dimensional world, which is a straight line, on which N cities are located, sequentially numbered from 0 to N - 1. The direction in the direction from the first city to the zero is called western, and in the opposite direction — eastern.
When the crisis suddenly began in Finland, all the inhabitants of the world began to experience deep confusion. Rumors began to circulate throughout Lapland that life is better in the east than in the west.
And so began the Great Line land Migration. The inhabitants of the world went to the east in whole cities, leaving their native streets, and moved until they came to a city in which the average price of living was less than in their native one.*

```javascript
const readline = require('readline');
const rl = readline.createInterface({
    input: process.stdin,
    output: process.stdout
});

function main(citys, prices) {
    prices = prices.split(' ');
    let result = prices;
    let stack = [];

    prices.forEach((item, index) => {
        item = Number(item);

        for (var i = stack.length - 1; i >= 0; i--) {
            if (item < stack[i][0]) {
                result[stack[i][1]] = index;
                stack.pop();
            } else {
                break;
            }
        }

        stack.push([item, index]);
    });

    stack.forEach(item => result[item[1]] = -1);


    console.log(result.join(' '));
}

rl.question('', (answer1) => {
    rl.question('', (answer2) => {
        main(answer1, answer2);
        rl.close();
    });
});
```
---

### Courses:

- Yandex Practicum Frontend Developer
- RS Schools Course «JavaScript/Front-end. Stage 1» (in progress)

---

### Languages:

- English \- Intermediate/Upper-intermediate
- Russian \- Native