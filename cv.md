# Kira Beloludinova 
---

![Альтернативный текст](https://i.imgur.com/hcdZH1Y.png)
## Contacts
- discord: KiraBelo(@KiraBelo)
- tg: @KiraBelo
- github: [my github](https://github.com/KiraBelo"there")

> Hi, I'm Kira. I am 34 years old and I am a js-developer. I am in love with javascript and really want to become a great programmer. 

## My skills
---

- **Javascript/ES5/S6**
- **Node.JS**
- **DOM API**
- **HTML/CSS3**
- **HTTP/HTTPS**
- **Git**
- **npm, yarn**
- **VIM/VScode**
- **LaTeX**


## My code example
---
> Implement and export a default function that takes a list of input companies (example list in _src/index.js_) and uses that list to generate positions (one for each company). Clicking on getting a company description (if there is a description of another company, it is replaced). Reappearance of conclusion. The data must be completely removed, hiding with classes is not suitable. By default, no description is shown.

```javascript
const app = (companies) => {
  const container = document.querySelector('div.container');
  let activeCompanyId = null;
  const render = (companies) => {
    container.textContent = '';
    companies.forEach((company) => {
      const button = document.createElement('button');
      button.className = 'btn btn-primary';
      button.textContent = company.name;
      const description = document.createElement('div');
      description.textContent = company.description;
      description.className = 'description';
      description.dataset.companyId = company.id;
      button.addEventListener('click', () => {
        if (activeCompanyId === company.id) {
          activeCompanyId = null;
         description.remove();
        } else {
          activeCompanyId = company.id;
          container.querySelectorAll('.description').forEach((el) => el.remove());
          container.appendChild(description);
        }
      });
      container.appendChild(button);
    });
  };
  render(companies);
};
export default app 
```

## Experience
---
### [Brain-games](https://github.com/KiraBelo/frontend-project-lvl1)
_5 math mini-games_
Skills:
- REPL
- npm, babel, eslint, makefile
- Airbnb
- Github


### [Difference calculator](https://github.com/KiraBelo/frontend-project-46.git)
_Utility for finding differences in configuration files._
Utility Features:
- _Support for different formats_
- _Generating a report in the form of plain text, pretty and json_
Skills:
- [commander.js](https://github.com/tj/commander.js/)
- [Jest](https://jestjs.io/)
- TDD
- npm, babel, eslint, makefile
- webpack

## Education
---
- Incomplete higher education in the field of history and medicine
- I am a professional tailor, so I can see the whole in disparate pieces
- [Hexlet school](hexlet.io) Java-script frontend developer

## Languages
---
- Russian C2
- English B2
- Italian A1
