//
//    **********************************************************************************************
//    **   /^(?=.*[a-z])       // at least one lowercase letter                                   **
//    **   (?=.*[A-Z])       // at least one uppercase letter                                     **
//    **   (?=.*\d)          // at least one digit                                                **
//    **   (?=.*[\W_])       // at least one special character (non-word character or underscore) ** 
//    **   .{8,}$/           // at least 8 characters total                                       **
//    **   const passwordRegex = /^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[\W_]).{8,}$/;              **    
//    **********************************************************************************************



let div = document.createElement('div')
let paragraph = document.createElement('p')
let message = document.createElement('p')
let contentent = document.createTextNode('enter the pasword')
var msgcontentent = document.createTextNode('X')
let input = document.createElement('input')
paragraph.appendChild(contentent)
div.appendChild(paragraph)
div.appendChild(input)
div.style.textAlign = 'center '



input.onkeyup = function(){
     message.innerHTML = ""
    const value = input.value;
    const hasUppercase = /[A-Z]/.test(value)
    let lowercase =/^(?=.*[a-z])/.test(value) 
    let special = /(?=.*[\W_])/.test(value)
    let degit= /(?=.*\d)/.test(value) 
   
     L = input.value.length
    console.log(L)
    if (L < 8){
        let msgcon= document.createTextNode('At Least 8 Charachters ')
        message.appendChild(msgcon)
        div.appendChild(message)
        message.style.color='red'
    }
    if(!hasUppercase){
        let msgcon= document.createTextNode('must contain at least one uppercase letter ')
        message.appendChild(msgcon)
        div.appendChild(message)
        message.style.color='red'

    }
    if(!lowercase){
        let msgcon= document.createTextNode('must contain at least one lowercase letter ')
        message.appendChild(msgcon)
        div.appendChild(message)
        message.style.color='red'

    }
    if(!special){
        let msgcon= document.createTextNode('must contain at least one special charachter letter ')
        message.appendChild(msgcon)
        div.appendChild(message)
        message.style.color='red'

    }
    if(!degit){
        let msgcon= document.createTextNode('must contain at least one degits letter ')
        message.appendChild(msgcon)
        div.appendChild(message)
        message.style.color='red'
    }
    else{
        let msgcon= document.createTextNode('Valid Paasword ')
        message.appendChild(msgcon)
        div.appendChild(message)
        message.style.color='green'
    }

}

document.body.appendChild(div)
