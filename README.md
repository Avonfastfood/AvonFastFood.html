# AvonFastFood
<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">

<title>Avon Fast Food</title>

<style>
*{
    box-sizing:border-box;
    -webkit-tap-highlight-color:transparent;
}

html{
    scroll-behavior:smooth;
}

body{
    margin:0;
    padding:0;
    font-family:Arial,sans-serif;
    background:#fff7ed;
    color:#222;
    overflow-x:hidden;
}

/* HEADER */

header{
    background:linear-gradient(135deg,#ff512f,#f09819);
    color:white;
    text-align:center;
    padding:22px 12px;
    border-radius:0 0 22px 22px;
    box-shadow:0 3px 12px rgba(0,0,0,.15);
}

header h1{
    margin:0;
    font-size:27px;
    font-weight:800;
}

header p{
    margin:7px 0 0;
    font-size:14px;
    line-height:1.5;
}

/* MAIN */

.container{
    width:100%;
    max-width:650px;
    margin:auto;
    padding:10px;
}

/* NOTICE */

.notice{
    background:#fff3cd;
    color:#856404;
    border:1.5px solid #ffc107;
    padding:13px 10px;
    border-radius:14px;
    margin:12px 0;
    text-align:center;
    font-size:14px;
    line-height:1.5;
}

/* MENU TITLE */

.menu-title{
    text-align:center;
    margin:20px 0 12px;
    font-size:23px;
}

/* FOOD CARD */

.card{
    background:#fff;
    border-radius:16px;
    margin:14px 0;
    overflow:hidden;
    box-shadow:0 3px 12px rgba(0,0,0,.12);
}

.card img{
    width:100%;
    height:165px;
    display:block;
    object-fit:cover;
}

.card-content{
    padding:12px;
}

.card h2{
    margin:0 0 10px;
    font-size:21px;
}

/* OPTION */

.option{
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:8px;
    background:#fff5ed;
    padding:10px;
    margin:8px 0;
    border-radius:11px;
    border:1px solid #ffe0cc;
    min-height:65px;
}

.option span{
    flex:1;
    font-size:14px;
    line-height:1.4;
}

.option strong{
    color:#d84315;
    font-size:16px;
}

/* ADD BUTTON */

.add{
    flex-shrink:0;
    background:#ff5722;
    color:white;
    border:0;
    border-radius:9px;
    padding:11px 15px;
    min-width:62px;
    font-size:15px;
    font-weight:bold;
    touch-action:manipulation;
}

.add:active{
    transform:scale(.94);
}

/* CART */

.cart{
    background:white;
    padding:14px;
    border-radius:16px;
    box-shadow:0 3px 12px rgba(0,0,0,.12);
    margin:20px 0;
}

.cart h2{
    margin:0 0 12px;
    font-size:21px;
}

.cart-item{
    display:flex;
    align-items:center;
    gap:7px;
    padding:10px 0;
    border-bottom:1px solid #eee;
    font-size:14px;
}

.item-info{
    flex:1;
    line-height:1.4;
}

.item-price{
    color:#d84315;
    font-weight:bold;
}

/* QUANTITY */

.qty{
    display:flex;
    align-items:center;
    gap:5px;
}

.qty button{
    width:32px;
    height:32px;
    border:0;
    border-radius:8px;
    font-size:18px;
    font-weight:bold;
}

.minus{
    background:#eee;
}

.plus{
    background:#ff5722;
    color:white;
}

.qty-number{
    min-width:20px;
    text-align:center;
    font-weight:bold;
}

/* REMOVE */

.remove{
    border:0;
    background:#e53935;
    color:white;
    border-radius:7px;
    padding:7px 8px;
    font-size:12px;
}

/* EMPTY */

.empty{
    text-align:center;
    color:#777;
    padding:10px 0;
    font-size:14px;
}

/* TOTAL */

.total{
    text-align:right;
    font-size:21px;
    font-weight:bold;
    margin-top:14px;
    color:#d84315;
    border-top:2px dashed #ddd;
    padding-top:12px;
}

/* CUSTOMER */

.customer-title{
    margin-top:22px !important;
}

.name-row{
    display:flex;
    gap:7px;
}

input{
    width:100%;
    padding:14px 11px;
    margin:5px 0;
    border:1px solid #ccc;
    border-radius:10px;
    font-size:16px;
    outline:none;
    background:#fff;
}

input:focus{
    border-color:#ff5722;
    box-shadow:0 0 0 2px rgba(255,87,34,.10);
}

/* CONFIRM */

.ok{
    width:100%;
    padding:15px;
    margin-top:12px;
    background:#128c7e;
    color:white;
    border:0;
    border-radius:11px;
    font-size:17px;
    font-weight:bold;
    touch-action:manipulation;
}

.ok:active{
    transform:scale(.98);
}

/* FOOTER */

footer{
    text-align:center;
    padding:22px 12px 35px;
    color:#666;
    font-size:14px;
    line-height:1.6;
}

/* VERY SMALL MOBILE */

@media(max-width:360px){

    header h1{
        font-size:24px;
    }

    .card img{
        height:145px;
    }

    .option span{
        font-size:13px;
    }

    .add{
        min-width:55px;
        padding:10px 11px;
    }

    .cart-item{
        font-size:13px;
    }

    .qty button{
        width:29px;
        height:29px;
    }

    .remove{
        padding:6px;
        font-size:11px;
    }
}

/* TABLET / BIG SCREEN */

@media(min-width:651px){

    .container{
        padding:15px;
    }

    .card img{
        height:210px;
    }
}
</style>
</head>

<body>

<header>

<h1>🍽️ Avon Fast Food</h1>

<p>😋 स्वाद ऐसा कि बार-बार खाने का मन करे!</p>

<p>
📍 India One ATM के बगल में,<br>
लक्ष्मनपुर, उत्तर प्रदेश, बलिया
</p>

</header>


<div class="container">

<!-- NOTICE -->

<div class="notice">

📢 <strong>IMPORTANT NOTICE</strong>

<br>

ऑनलाइन ऑर्डर करने पर आपको ऑर्डर
<strong>दुकान से ही लेना होगा।</strong>

<br>

धन्यवाद ❤️

</div>


<!-- MENU -->

<h2 class="menu-title">🍴 हमारा मेन्यू</h2>


<!-- MOMO -->

<div class="card">

<img
src="https://images.unsplash.com/photo-1625220194771-7ebdea0b70b9?auto=format&fit=crop&w=900&q=80"
alt="Momo">

<div class="card-content">

<h2>🥟 Momo</h2>


<div class="option">

<span>
Veg Momo - Half (4 पीस)<br>
<strong>₹25</strong>
</span>

<button class="add"
onclick="addItem('Veg Momo Half (4 pcs)',25)">
Add
</button>

</div>


<div class="option">

<span>
Veg Momo - Full (8 पीस)<br>
<strong>₹50</strong>
</span>

<button class="add"
onclick="addItem('Veg Momo Full (8 pcs)',50)">
Add
</button>

</div>


<div class="option">

<span>
Soya Momo - Half (4 पीस)<br>
<strong>₹20</strong>
</span>

<button class="add"
onclick="addItem('Soya Momo Half (4 pcs)',20)">
Add
</button>

</div>


<div class="option">

<span>
Soya Momo - Full (8 पीस)<br>
<strong>₹40</strong>
</span>

<button class="add"
onclick="addItem('Soya Momo Full (8 pcs)',40)">
Add
</button>

</div>


<div class="option">

<span>
Paneer Momo - Half (4 पीस)<br>
<strong>₹30</strong>
</span>

<button class="add"
onclick="addItem('Paneer Momo Half (4 pcs)',30)">
Add
</button>

</div>


<div class="option">

<span>
Paneer Momo - Full (8 पीस)<br>
<strong>₹60</strong>
</span>

<button class="add"
onclick="addItem('Paneer Momo Full (8 pcs)',60)">
Add
</button>

</div>

</div>
</div>


<!-- CHOWMIN -->

<div class="card">

<img
src="https://images.unsplash.com/photo-1585032226651-759b368d7246?auto=format&fit=crop&w=900&q=80"
alt="Chowmin">

<div class="card-content">

<h2>🍜 Chowmin</h2>


<div class="option">

<span>
Chowmin - Half<br>
<strong>₹20</strong>
</span>

<button class="add"
onclick="addItem('Chowmin Half',20)">
Add
</button>

</div>


<div class="option">

<span>
Chowmin - Full<br>
<strong>₹30</strong>
</span>

<button class="add"
onclick="addItem('Chowmin Full',30)">
Add
</button>

</div>

</div>
</div>


<!-- IDLI -->

<div class="card">

<img
src="https://images.unsplash.com/photo-1589301760014-d929f3979dbc?auto=format&fit=crop&w=900&q=80"
alt="Idli">

<div class="card-content">

<h2>🍘 Idli</h2>


<div class="option">

<span>
Idli - 4 पीस<br>
<strong>₹30</strong>
</span>

<button class="add"
onclick="addItem('Idli (4 pcs)',30)">
Add
</button>

</div>

</div>
</div>


<!-- CART -->

<div class="cart" id="cartBox">

<h2>🛒 आपका Cart</h2>

<div id="cartItems">

<p class="empty">
अभी कोई item नहीं जोड़ा गया है।
</p>

</div>

<div class="total">
Total: ₹<span id="total">0</span>
</div>


<!-- CUSTOMER -->

<h2 class="customer-title">
👤 Customer Details
</h2>


<div class="name-row">

<input
id="firstName"
type="text"
placeholder="First Name"
autocomplete="given-name">

<input
id="lastName"
type="text"
placeholder="Last Name"
autocomplete="family-name">

</div>


<input
id="mobile"
type="tel"
inputmode="numeric"
maxlength="10"
placeholder="10 अंकों का Mobile Number"
oninput="this.value=this.value.replace(/[^0-9]/g,'').slice(0,10)"
autocomplete="tel">


<button
class="ok"
onclick="confirmOrder()">

✅ OK - Order Confirm करें

</button>

</div>

</div>


<footer>

<strong>Avon Fast Food</strong>

<br>

📍 India One ATM के बगल में,
लक्ष्मनपुर, उत्तर प्रदेश, बलिया

<br><br>

धन्यवाद ❤️

</footer>


<script>

let cart = [];


/* ADD ITEM */

function addItem(name,price){

    let existing = cart.find(
        item => item.name === name
    );

    if(existing){

        existing.qty++;

    }else{

        cart.push({
            name:name,
            price:price,
            qty:1
        });

    }

    showCart();

    setTimeout(function(){

        document.getElementById("cartBox")
        .scrollIntoView({
            behavior:"smooth",
            block:"center"
        });

    },100);
}


/* CALCULATE TOTAL */

function calculateTotal(){

    return cart.reduce(function(sum,item){

        return sum + (item.price * item.qty);

    },0);
}


/* SHOW CART */

function showCart(){

    const box =
    document.getElementById("cartItems");

    const total =
    calculateTotal();

    document.getElementById("total").innerText =
    total;


    if(cart.length === 0){

        box.innerHTML =
        '<p class="empty">अभी कोई item नहीं जोड़ा गया है।</p>';

        return;
    }


    box.innerHTML = "";


    cart.forEach(function(item,index){

        box.innerHTML += `

        <div class="cart-item">

            <div class="item-info">

                <b>${index+1}. ${item.name}</b>

                <br>

                <span class="item-price">
                ₹${item.price} × ${item.qty}
                </span>

            </div>


            <div class="qty">

                <button
                class="minus"
                onclick="changeQty(${index},-1)">
                −
                </button>

                <span class="qty-number">
                ${item.qty}
                </span>

                <button
                class="plus"
                onclick="changeQty(${index},1)">
                +
                </button>

            </div>


            <button
            class="remove"
            onclick="removeItem(${index})">
            ❌
            </button>

        </div>

        `;

    });

}


/* CHANGE QUANTITY */

function changeQty(index,value){

    cart[index].qty += value;


    if(cart[index].qty <= 0){

        cart.splice(index,1);

    }


    showCart();
}


/* REMOVE ITEM */

function removeItem(index){

    cart.splice(index,1);

    showCart();

}


/* CONFIRM ORDER */

function confirmOrder(){

    if(cart.length === 0){

        alert("पहले कोई Food Item चुनें।");

        return;
    }


    let firstName =
    document.getElementById("firstName")
    .value.trim();


    let lastName =
    document.getElementById("lastName")
    .value.trim();


    let mobile =
    document.getElementById("mobile")
    .value.trim();


    if(firstName === ""){

        alert("कृपया First Name लिखें।");

        document.getElementById("firstName").focus();

        return;
    }


    if(lastName === ""){

        alert("कृपया Last Name लिखें।");

        document.getElementById("lastName").focus();

        return;
    }


    if(mobile.length !== 10){

        alert(
        "Mobile Number ठीक 10 अंकों का होना चाहिए।"
        );

        document.getElementById("mobile").focus();

        return;
    }


    let customerName =
    firstName + " " + lastName;


    let total =
    calculateTotal();


    /*
       WhatsApp Message
    */

    let message =
    "🍽️ *AVON FAST FOOD ORDER*\n\n";


    message +=
    "👤 Name: " +
    customerName +
    "\n";


    message +=
    "📱 Mobile: " +
    mobile +
    "\n\n";


    message +=
    "🛒 *ORDER DETAILS*\n";


    cart.forEach(function(item,index){

        message +=
        (index+1) +
        ". " +
        item.name +
        " × " +
        item.qty +
        " = ₹" +
        (item.price * item.qty) +
        "\n";

    });


    message +=
    "\n💰 *TOTAL: ₹" +
    total +
    "*\n\n";


    message +=
    "📍 *Pickup Address:*\n" +
    "India One ATM के बगल में,\n" +
    "लक्ष्मनपुर, उत्तर प्रदेश, बलिया";


    /*
       WhatsApp Number
    */

    const whatsappNumber =
    "919682816332";


    const whatsappURL =
    "https://wa.me/" +
    whatsappNumber +
    "?text=" +
    encodeURIComponent(message);


    /*
       FINAL CONFIRM
    */

    if(
        confirm(
        "क्या आप अपना Order Confirm करके WhatsApp पर भेजना चाहते हैं?"
        )
    ){

        window.location.href =
        whatsappURL;

    }

}

</script>

</body>
</html>
