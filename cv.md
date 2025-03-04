# Darya Babich
<img src="cv.png" alt="My-photo" width="160">

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
- **TypeScript**
- Version control: **Git** (**GitHub** remote service)
- Development tools: **VSCode**
- Module bundlers: **Webpack**
- CSS pre-processors: **Sass**
- Figma, Illustrator as an auxiliary tools

## Code Examples
```
class News {
    public draw(data: INewsApiArticles[]): void {
        const news: INewsApiArticles[] = data.length >= 10 ? data.filter((_item, idx) => idx < 10) : data;

        const fragment: DocumentFragment = document.createDocumentFragment();
        const newsItemTemp: querySelectorType = document.querySelector('#newsItemTemp');
        if (!(newsItemTemp instanceof HTMLTemplateElement)) {
            console.error('error');
            return;
        }

        news.forEach((item, idx) => {
            const newsClone = newsItemTemp.content.cloneNode(true);
            if (!(newsClone instanceof DocumentFragment)) {
                console.error('error');
                return;
            }

            if (idx % 2) {
                const newsItem: querySelectorType = newsClone.querySelector('.news__item');
                if (newsItem) {
                    // newsItem.classList.add('alt');
                    newsItem.classList.add(ENewsItemStyle.Alt);
                }
            }

            const metaPhoto: querySelectorType = newsClone.querySelector('.news__meta-photo');
            if (metaPhoto instanceof HTMLElement) {
                metaPhoto.style.backgroundImage = `url(${item.urlToImage || 'img/news_placeholder.jpg'})`;
            }
            const metaAuthor: querySelectorType = newsClone.querySelector('.news__meta-author');
            if (metaAuthor) {
                metaAuthor.textContent = item.author || item.source.name;
            }

            const metaDate: querySelectorType = newsClone.querySelector('.news__meta-date');
            if (metaDate) {
                metaDate.textContent = item.publishedAt.slice(0, 10).split('-').reverse().join('-');
            }

            const descriptionTitle: querySelectorType = newsClone.querySelector('.news__description-title');
            if (descriptionTitle) {
                descriptionTitle.textContent = item.title;
            }
            const descriptionSource: htmlElementType = getElement<HTMLElement>(newsClone, '.news__description-source');
            if (descriptionSource) {
                descriptionSource.textContent = item.source.name;
            }
            const descriptionContent: htmlElementType = getElement<HTMLElement>(
                newsClone,
                '.news__description-content'
            );
            if (descriptionContent) {
                descriptionContent.textContent = item.description;
            }
            const readMore: htmlElementType = getElement<HTMLElement>(newsClone, '.news__read-more a');
            if (readMore) {
                readMore.setAttribute('href', item.url);
            }

            fragment.append(newsClone);
        });

        const newsContainer: querySelectorType = document.querySelector('.news');
        if (newsContainer instanceof HTMLElement) {
            newsContainer.innerHTML = '';
            newsContainer.appendChild(fragment);
        }
    }
}
```

## Work Experience
**ʕᵔᴥᵔʔ**
- [CV](https://github.com/dashulinushka/rsschool-cv/blob/gh-pages/cv.md)
- [HTML-builder](https://github.com/dashulinushka/HTML-builder)
- [Core-js-arrays](https://github.com/dashulinushka/core-js-arrays)
Also translated a small project from **JS** to **TS** and other things
**ʕᵔᴥᵔʔ** 


## Education
* **Belarusian State University of Informatics and Radioelectronics**:
    * a *programmer-economist*
    * a *third* year student
    * average score *9.28/10*
    * the expected date of graduation *July 2026*

## Languages
### Native
- Russian
- Belorussian
### Foreign
- English **A2-B1**
- German **A2**