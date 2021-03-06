# Disclose file format of links
author: catalin

levels:

  - medium

type: normal

category: how to

links:

  - >-
    [css-tricks.com](https://css-tricks.com/almanac/properties/c/content/){website}

---
## Content

To indicate what type a download link is (such as a `doc` or a `pdf`) via an image, use the **CSS** `content` property.


```css
[href$=".pdf"]::after{
content: url("myImgUrl.png");
}

```

The code snippet above will display at the end of any link ending on `.pdf` (any link to a pdf file), with the help of `::after` selector the image hosted at `myImgUrl.png`.

![HtmlToSvgmin.svg](%3Csvg%20height=%22auto%22%20viewBox=%220%200%20800%20300%22%20xmlns=%22http://www.w3.org/2000/svg%22%20version=%221.2%22%20baseProfile=%22tiny%22%3E%3Cdesc%3ECreated%20by%20HiQPdf%3C/desc%3E%3Cg%20fill=%22none%22%20stroke=%22#000%22%20fill-rule=%22evenodd%22%20stroke-linecap=%22square%22%20stroke-linejoin=%22bevel%22%3E%3Cpath%20d=%22M8%208h800v300H8V8%22%20fill=%22#596193%22%20stroke=%22none%22/%3E%3Ctext%20stroke=%22none%22%20x=%22298%22%20y=%22103%22%20font-family=%22Arial%22%20font-size=%2260%22%20font-weight=%22400%22%20fill=%22#fff%22%3ENormal%20link%3C/text%3E%3Cpath%20fill=%22none%22%20d=%22M298%20104.5h297%22%20stroke=%22#fff%22%20stroke-linejoin=%22miter%22%20stroke-miterlimit=%222%22/%3E%3Ctext%20stroke=%22none%22%20x=%22298%22%20y=%22232%22%20font-family=%22Arial%22%20font-size=%2260%22%20font-weight=%22400%22%20fill=%22#fff%22%3EPdf%20link%3C/text%3E%3Cpath%20fill=%22none%22%20d=%22M298%20233.5h196%22%20stroke=%22#fff%22%20stroke-linejoin=%22miter%22%20stroke-miterlimit=%222%22/%3E%3Cpath%20fill-rule=%22nonzero%22%20d=%22M521.313%20218.42c-.427-.42-1.372-.642-2.812-.66-.973-.012-2.146.074-3.38.247-.55-.32-1.12-.665-1.567-1.083-1.202-1.122-2.205-2.68-2.83-4.394.04-.16.074-.3.107-.444%200%200%20.677-3.846.498-5.146-.025-.178-.04-.23-.088-.37l-.06-.15c-.183-.425-.544-.875-1.11-.85l-.34-.01c-.632%200-1.147.322-1.282.804-.41%201.514.013%203.778.78%206.71l-.196.48c-.55%201.34-1.238%202.688-1.846%203.88l-.08.154c-.638%201.25-1.22%202.313-1.744%203.213l-.543.288c-.04.02-.97.513-1.19.645-1.85%201.106-3.078%202.36-3.28%203.357-.066.318-.018.725.312.913l.525.264c.228.114.468.172.714.172%201.32%200%202.85-1.644%204.96-5.325%202.435-.793%205.208-1.452%207.638-1.815%201.852%201.043%204.13%201.767%205.567%201.767.255%200%20.475-.024.654-.072.275-.073.507-.23.65-.444.278-.42.334-.997.26-1.59-.024-.175-.164-.392-.316-.54m-19.7%207.02c.24-.66%201.192-1.96%202.6-3.112.088-.072.306-.276.506-.466-1.472%202.348-2.458%203.283-3.106%203.577m8.337-19.2c.425%200%20.666%201.07.686%202.07.02%201-.214%201.705-.505%202.225-.24-.77-.356-1.984-.356-2.778%200%200-.018-1.517.177-1.517m-2.486%2013.682c.295-.53.603-1.086.917-1.677.766-1.447%201.25-2.58%201.61-3.51.716%201.302%201.608%202.41%202.656%203.296.13.112.27.223.415.334-2.13.422-3.973.935-5.595%201.558m13.438-.12c-.13.08-.502.128-.74.128-.773%200-1.728-.353-3.067-.927.515-.038.986-.057%201.41-.057.773%200%201.003-.003%201.76.19.757.193.767.585.637.667%22%20fill=%22#fff%22%20stroke=%22none%22/%3E%3Cpath%20fill-rule=%22nonzero%22%20d=%22M523.68%20207.16c-.693-.948-1.66-2.054-2.723-3.117-1.062-1.063-2.17-2.03-3.116-2.724-1.61-1.183-2.392-1.32-2.84-1.32h-15.5c-1.378%200-2.5%201.12-2.5%202.5v27c0%201.378%201.12%202.5%202.5%202.5h23c1.378%200%202.5-1.122%202.5-2.5V210c0-.448-.137-1.23-1.32-2.84m-4.137-1.703c.96.96%201.712%201.825%202.268%202.543H517v-4.81c.718.555%201.584%201.308%202.543%202.267M523%20229.5c0%20.27-.23.5-.5.5h-23c-.27%200-.5-.23-.5-.5v-27c0-.27.23-.5.5-.5H515v7c0%20.552.448%201%201%201h7v19.5%22%20fill=%22#fff%22%20stroke=%22none%22/%3E%3C/g%3E%3C/svg%3E)

---
## Revision

A CSS selector that targets links which resolve to a *pdf* file is:

???

* `a[href$=".pdf"]`
* `a.pdf`
* `[href="pdf"]`
* `a[after=".pdf"]`
