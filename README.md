# Capgemini---Front-end-Software-Engineering-Track
Capgemini - Front-end Software Engineering Track      
//// Fetching data from objects into html

const objArticle = document.getElementById('objectArticle');
// const objHeader = document.getElementById('objectTitle');
// const objText = document.getElementById('objText');



const postArr = [
    {
        post: 'theFirstPost',
        postText: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. '
    },
    {
        post: 'theSndPost',
        postText: 'Iure sunt animi officiis unde aspernatur sequi recusandae.'
    },
    {
        post: 'theThirdPost',
        postText: 'Harum voluptate exercitationem autem aliquam explicabo.'
    },
    {
        post: 'theFourthPost',
        postText: 'Nobis, fugit provident!'
    
    },
    {
        post: 'theFifthPost',
        postText: 'Odit tempora harum hic iste.'
    }
]



const hopeItWorks = postArr.map(item => {
return `<h1>${item.post}</h1>
<p>${item.postText}</p>`


}).join('');
objArticle.innerHTML = hopeItWorks;
// console.log(postArr);

for(let post of postArr) {
    objArticle.innerHTML += post.post;
}


