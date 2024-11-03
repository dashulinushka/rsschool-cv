# Darya Babich

## Contact Information
- **Address**: Minsk, Belarus 
- **E-mail**: [darya.babich11@gmail.com](https://darya.babich11@gmail.com)
- **LinkedIn**: [darya-babich](https://www.linkedin.com/in/darya-babich)
- **Discord**: dashulinushka

## Self-Introduction
I am currently studying at BSUIR as a *programmer-economist* in the 3rd year. I am interested in further training on *frontend developer*. There is a great desire to get *new knowledge and master technologies* in this direction. At the moment, *the main goal* is to learn the *Java Script*, as well as the *React* framework

## Skills
- **HTML**
- **CSS**
- **JavaScript**
- Version control: **Git** (**GitHub** remote service)
- Development tools: **VSCode**
- Figma, Illustrator as an auxiliary tool

## Code Examples
```
function arrayDiff(a, b) {
  // wrong: for (let i = 0; i < a.length; i++){}
  // wrong: return a.filter(item => item!=b)
  // wrong: return a.filter(item => item.a!=b)
  // wrong: return a.filter(item => !item.b)
  // right return a.filter(item => !b.includes(item));
  let result = [];
  
  for (let item of a){
    let isB = false;
    
    for (let elem of b){
      if(item === elem){
        isB = true;
        break;
      }
    }
    
    if (!isB){
      result.push(item);
    }
  }
  
  return result;
}
```

## Work Experience
**ʕᵔᴥᵔʔ** *currently unavailable* **ʕᵔᴥᵔʔ**
            *will appear later*

## Education
* Belarusian State University of Informatics and Radioelectronics:
    * a *programmer-economist*
    * a *third* year student
    * average score *9.28/10*
    * the expected date of graduation July *2026*