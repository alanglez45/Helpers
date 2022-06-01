# **Helpers Programming**

## **Regular Expressions**
### Email

    /^(([^<>()\[\]\\.,;:\s@"]+(\.[^<>()\[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/

[For other languages](https://emailregex.com/)

### Proper names

    /^([A-ZÁÉÍÓÚ]{1}[a-zñáéíóú]+[\s]*)+$/

[Other expressions](https://aprende-web.net/javascript/js13_3.php)

    
## **ID Generator**
    //generates random id;
    let guid = () => {
        let s4 = () => {
            return Math.floor((1 + Math.random()) * 0x10000)
                .toString(16)
                .substring(1);
        }
        //return id of format 'aaaaaaaa'-'aaaa'-'aaaa'-'aaaa'-'aaaaaaaaaaaa'
        return s4() + s4() + '-' + s4() + '-' + s4() + '-' + s4() + '-' + s4() + s4() + s4();
    }

    console.log(guid());
    //"c2181edf-041b-0a61-3651-79d671fa3db7"

[URL](https://learnersbucket.com/examples/javascript/unique-id-generator-in-javascript/#:~:text=Javascript%20does%20not%20have%20any,to%20generate%20unique%20random%20ids)