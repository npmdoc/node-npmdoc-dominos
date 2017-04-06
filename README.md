# api documentation for  [dominos (v2.1.1)](https://github.com/RIAEvangelist/node-dominos-pizza-api)  [![npm package](https://img.shields.io/npm/v/npmdoc-dominos.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-dominos) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-dominos.svg)](https://travis-ci.org/npmdoc/node-npmdoc-dominos)
#### node js API for Domino's pizza

[![NPM](https://nodei.co/npm/dominos.png?downloads=true)](https://www.npmjs.com/package/dominos)

[![apidoc](https://npmdoc.github.io/node-npmdoc-dominos/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-dominos_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-dominos/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-dominos/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-dominos/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Brandon Miller",
        "email": "brandon@diginow.it"
    },
    "bugs": {
        "url": "https://github.com/RIAEvangelist/node-dominos-pizza-api/issues"
    },
    "contributors": [
        {
            "name": "Julian Hartline",
            "email": "julianh2o@gmail.com",
            "url": "http://www.julianhartline.com"
        },
        {
            "name": "Madeline Cameron",
            "email": "madeline@madelinecameron.net",
            "url": "http://madelinecameron.net"
        },
        {
            "name": "Adrian Sida"
        },
        {
            "name": "Victor Quinn"
        },
        {
            "name": "Matt Cotter"
        }
    ],
    "dependencies": {
        "request": "^2.50.0",
        "xml2json": "^0.9.0"
    },
    "description": "node js API for Domino's pizza",
    "devDependencies": {
        "chai": "^3.0.0",
        "colors": "^1.0.3",
        "mocha": "^2.2.5"
    },
    "directories": {
        "example": "example"
    },
    "dist": {
        "shasum": "64cd3700265df04a6f6aca4113434e1353c2318b",
        "tarball": "https://registry.npmjs.org/dominos/-/dominos-2.1.1.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "gitHead": "52ab1b6d41baa53a2190db97234ba6a8f6abb683",
    "homepage": "https://github.com/RIAEvangelist/node-dominos-pizza-api",
    "keywords": [
        "Dominos",
        "Domino's",
        "Pizza",
        "API",
        "Pie",
        "PizzaPI"
    ],
    "license": "DBAD",
    "main": "dominos-pizza-api.js",
    "maintainers": [
        {
            "name": "madeline",
            "email": "madeline@madelinecameron.net"
        },
        {
            "name": "pdube",
            "email": "patrickdube91@gmail.com"
        },
        {
            "name": "riaevangelist",
            "email": "brandon@diginow.it"
        },
        {
            "name": "sgnl",
            "email": "npm@rayfarias.com"
        },
        {
            "name": "victorquinn",
            "email": "mail@victorquinn.com"
        }
    ],
    "name": "dominos",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/RIAEvangelist/node-dominos-pizza-api.git"
    },
    "scripts": {
        "start": "node example/commandline-pizza/dominos-commandline-pizza.js",
        "test": "mocha"
    },
    "version": "2.1.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module dominos](#apidoc.module.dominos)
1.  [function <span class="apidocSignatureSpan">dominos.</span>Address (parameters)](#apidoc.element.dominos.Address)
1.  [function <span class="apidocSignatureSpan">dominos.</span>Coupon (parameters)](#apidoc.element.dominos.Coupon)
1.  [function <span class="apidocSignatureSpan">dominos.</span>Customer (parameters)](#apidoc.element.dominos.Customer)
1.  [function <span class="apidocSignatureSpan">dominos.</span>Item (parameters)](#apidoc.element.dominos.Item)
1.  [function <span class="apidocSignatureSpan">dominos.</span>Menu (menuData)](#apidoc.element.dominos.Menu)
1.  [function <span class="apidocSignatureSpan">dominos.</span>MenuCategory (menuData, parentCategory)](#apidoc.element.dominos.MenuCategory)
1.  [function <span class="apidocSignatureSpan">dominos.</span>MenuItem (menuData)](#apidoc.element.dominos.MenuItem)
1.  [function <span class="apidocSignatureSpan">dominos.</span>Order (parameters)](#apidoc.element.dominos.Order)
1.  [function <span class="apidocSignatureSpan">dominos.</span>Store (parameters)](#apidoc.element.dominos.Store)
1.  object <span class="apidocSignatureSpan">dominos.</span>Menu.prototype
1.  object <span class="apidocSignatureSpan">dominos.</span>MenuCategory.prototype
1.  object <span class="apidocSignatureSpan">dominos.</span>MenuItem.prototype
1.  object <span class="apidocSignatureSpan">dominos.</span>Order.prototype
1.  object <span class="apidocSignatureSpan">dominos.</span>Store.prototype
1.  object <span class="apidocSignatureSpan">dominos.</span>Track
1.  object <span class="apidocSignatureSpan">dominos.</span>Util
1.  object <span class="apidocSignatureSpan">dominos.</span>http_json

#### [module dominos.Menu](#apidoc.module.dominos.Menu)
1.  [function <span class="apidocSignatureSpan">dominos.</span>Menu (menuData)](#apidoc.element.dominos.Menu.Menu)

#### [module dominos.Menu.prototype](#apidoc.module.dominos.Menu.prototype)
1.  [function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>buildCategories (categoryData, parent)](#apidoc.element.dominos.Menu.prototype.buildCategories)
1.  [function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>getCouponCategory ()](#apidoc.element.dominos.Menu.prototype.getCouponCategory)
1.  [function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>getFoodCategory ()](#apidoc.element.dominos.Menu.prototype.getFoodCategory)
1.  [function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>getItemByCode (code)](#apidoc.element.dominos.Menu.prototype.getItemByCode)
1.  [function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>getPreconfiguredCategory ()](#apidoc.element.dominos.Menu.prototype.getPreconfiguredCategory)
1.  [function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>getRaw ()](#apidoc.element.dominos.Menu.prototype.getRaw)
1.  [function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>parseItems (parentMenuData, ParseClass)](#apidoc.element.dominos.Menu.prototype.parseItems)
1.  [function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>parseMenu (menuData)](#apidoc.element.dominos.Menu.prototype.parseMenu)

#### [module dominos.MenuCategory](#apidoc.module.dominos.MenuCategory)
1.  [function <span class="apidocSignatureSpan">dominos.</span>MenuCategory (menuData, parentCategory)](#apidoc.element.dominos.MenuCategory.MenuCategory)

#### [module dominos.MenuCategory.prototype](#apidoc.module.dominos.MenuCategory.prototype)
1.  [function <span class="apidocSignatureSpan">dominos.MenuCategory.prototype.</span>getCategoryPath ()](#apidoc.element.dominos.MenuCategory.prototype.getCategoryPath)
1.  [function <span class="apidocSignatureSpan">dominos.MenuCategory.prototype.</span>getCode ()](#apidoc.element.dominos.MenuCategory.prototype.getCode)
1.  [function <span class="apidocSignatureSpan">dominos.MenuCategory.prototype.</span>getDescription ()](#apidoc.element.dominos.MenuCategory.prototype.getDescription)
1.  [function <span class="apidocSignatureSpan">dominos.MenuCategory.prototype.</span>getName ()](#apidoc.element.dominos.MenuCategory.prototype.getName)
1.  [function <span class="apidocSignatureSpan">dominos.MenuCategory.prototype.</span>getProducts ()](#apidoc.element.dominos.MenuCategory.prototype.getProducts)
1.  [function <span class="apidocSignatureSpan">dominos.MenuCategory.prototype.</span>getSubcategories ()](#apidoc.element.dominos.MenuCategory.prototype.getSubcategories)

#### [module dominos.MenuItem](#apidoc.module.dominos.MenuItem)
1.  [function <span class="apidocSignatureSpan">dominos.</span>MenuItem (menuData)](#apidoc.element.dominos.MenuItem.MenuItem)

#### [module dominos.MenuItem.prototype](#apidoc.module.dominos.MenuItem.prototype)
1.  [function <span class="apidocSignatureSpan">dominos.MenuItem.prototype.</span>getCategories ()](#apidoc.element.dominos.MenuItem.prototype.getCategories)
1.  [function <span class="apidocSignatureSpan">dominos.MenuItem.prototype.</span>getCode ()](#apidoc.element.dominos.MenuItem.prototype.getCode)
1.  [function <span class="apidocSignatureSpan">dominos.MenuItem.prototype.</span>getDescription ()](#apidoc.element.dominos.MenuItem.prototype.getDescription)
1.  [function <span class="apidocSignatureSpan">dominos.MenuItem.prototype.</span>getName ()](#apidoc.element.dominos.MenuItem.prototype.getName)
1.  [function <span class="apidocSignatureSpan">dominos.MenuItem.prototype.</span>setCategories (categories)](#apidoc.element.dominos.MenuItem.prototype.setCategories)

#### [module dominos.Order](#apidoc.module.dominos.Order)
1.  [function <span class="apidocSignatureSpan">dominos.</span>Order (parameters)](#apidoc.element.dominos.Order.Order)

#### [module dominos.Order.prototype](#apidoc.module.dominos.Order.prototype)
1.  [function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>PaymentObject ()](#apidoc.element.dominos.Order.prototype.PaymentObject)
1.  [function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>addCoupon (Coupon)](#apidoc.element.dominos.Order.prototype.addCoupon)
1.  [function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>addItem (Item)](#apidoc.element.dominos.Order.prototype.addItem)
1.  [function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>mergeResponse (callback, response)](#apidoc.element.dominos.Order.prototype.mergeResponse)
1.  [function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>place (callback)](#apidoc.element.dominos.Order.prototype.place)
1.  [function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>price (callback)](#apidoc.element.dominos.Order.prototype.price)
1.  [function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>removeCoupon (Coupon)](#apidoc.element.dominos.Order.prototype.removeCoupon)
1.  [function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>removeItem (Item)](#apidoc.element.dominos.Order.prototype.removeItem)
1.  [function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>validate (callback)](#apidoc.element.dominos.Order.prototype.validate)
1.  [function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>validateCC (number)](#apidoc.element.dominos.Order.prototype.validateCC)

#### [module dominos.Store](#apidoc.module.dominos.Store)
1.  [function <span class="apidocSignatureSpan">dominos.</span>Store (parameters)](#apidoc.element.dominos.Store.Store)

#### [module dominos.Store.prototype](#apidoc.module.dominos.Store.prototype)
1.  [function <span class="apidocSignatureSpan">dominos.Store.prototype.</span>getFriendlyNames (callback, lang)](#apidoc.element.dominos.Store.prototype.getFriendlyNames)
1.  [function <span class="apidocSignatureSpan">dominos.Store.prototype.</span>getInfo (callback)](#apidoc.element.dominos.Store.prototype.getInfo)
1.  [function <span class="apidocSignatureSpan">dominos.Store.prototype.</span>getMenu (callback, lang, noCache)](#apidoc.element.dominos.Store.prototype.getMenu)

#### [module dominos.Track](#apidoc.module.dominos.Track)
1.  [function <span class="apidocSignatureSpan">dominos.Track.</span>byId (storeID, orderKey, callback)](#apidoc.element.dominos.Track.byId)
1.  [function <span class="apidocSignatureSpan">dominos.Track.</span>byPhone (phone, callback)](#apidoc.element.dominos.Track.byPhone)
1.  [function <span class="apidocSignatureSpan">dominos.Track.</span>byUrl (url, callback)](#apidoc.element.dominos.Track.byUrl)

#### [module dominos.Util](#apidoc.module.dominos.Util)
1.  [function <span class="apidocSignatureSpan">dominos.Util.</span>findNearbyStores (address, pickUpType, callback)](#apidoc.element.dominos.Util.findNearbyStores)

#### [module dominos.http_json](#apidoc.module.dominos.http_json)
1.  [function <span class="apidocSignatureSpan">dominos.http_json.</span>get (url, callback)](#apidoc.element.dominos.http_json.get)
1.  [function <span class="apidocSignatureSpan">dominos.http_json.</span>post (url, req, callback)](#apidoc.element.dominos.http_json.post)



# <a name="apidoc.module.dominos"></a>[module dominos](#apidoc.module.dominos)

#### <a name="apidoc.element.dominos.Address"></a>[function <span class="apidocSignatureSpan">dominos.</span>Address (parameters)](#apidoc.element.dominos.Address)
- description and source-code
```javascript
Address = function (parameters) {
    Object.defineProperties(
        this,
        {
            parse:{
                value:parse,
                enumerable:true,
                writable:false
            },
            getAddressLines:{
                value:getAddressLines,
                enumerable:true,
                writable:false
            },
            Type:{
                value:'House',
                enumerable:true,
                writable:true
            },
            Street:{
                value:'',
                enumerable:true,
                writable:true
            },
            City:{
                value:'',
                enumerable:true,
                writable:true
            },
            Region:{
                value:'',
                enumerable:true,
                writable:true
            },
            PostalCode:{
                value:'',
                enumerable:true,
                writable:true
            },
            _init:{
                value:init,
                enumerable:false,
                writable:false
            },
            _parameters:{
                value:parameters,
                enumerable:false,
                writable:false
            }
        }
    );

    this._init();

    function init(){
        if (typeof this._parameters == 'object' && this._parameters.PostalCode) {
            this.Street = this._parameters.Street;
            this.City = this._parameters.City;
            this.Region = this._parameters.Region;
            this.PostalCode = this._parameters.PostalCode;
        }



        if (util.isArray(this._parameters)) {
            this.Street = this._parameters[0];
            this.City = this._parameters[1];
            this.Region = this._parameters[2];
            this.PostalCode = this._parameters[3];
        }

        if (typeof this._parameters == 'number') {
            this._parameters+='';
        }

        if (typeof this._parameters == 'string') {
            this.parse(this._parameters);
        }

        if (this._parameters.Type) {
            this.Type = this._parameters.Type;
        }
    }

    function parse(locationString) {
        var splitAddress = locationString.split(',');

        for (var i in splitAddress) {
            splitAddress[i] = splitAddress[i].trim();
        }

        this.PostalCode= splitAddress[splitAddress.length-1]

        //need better intellegence for auto determining address parts
        //added some, should externalize it
        //while not perfect, it does seem to get most of the right stuff
        //in good enough places for dominos to like it.
        switch (splitAddress.length) {
            case 1:
                if (!this.PostalCode) {
                    this.PostalCode='';
                    this.City = splitAddress[0];
                }
                break;
            case 2:
                if(splitAddress[0].length<3){
                    this.Region = splitAddress[0];
                }else{
                    this.City = splitAddress[0];
                }
                if (!this.PostalCode) {
                    if(splitAddress[1].length>2){
                        if(this.City){
                            this.Street = this.City;
                        }
                        this.City = splitAddress[1];
                    }else{
                        if(this.Region){
                            this.City=this.Region;
                        }
                        this.Region = splitAddress[1];
                    }
                }
                break;
            case 3:
                if(splitAddress[0].length<3){
                    this.Region = splitAddress[0];
                }else{
                    this.City = splitAddress[0];
                }

                if(splitAddress[1].length<3){
                    if(this.Region){
                        if(this.City){
                            this.Street = this.City;
                        }
                        this.City=this.Region;
                    } ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.Coupon"></a>[function <span class="apidocSignatureSpan">dominos.</span>Coupon (parameters)](#apidoc.element.dominos.Coupon)
- description and source-code
```javascript
Coupon = function (parameters) {
    this.Code = parameters.code;
    this.Qty = parameters.quantity ? parameters.quantity : 1;
    this.ID = 1;
    this.isNew = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.Customer"></a>[function <span class="apidocSignatureSpan">dominos.</span>Customer (parameters)](#apidoc.element.dominos.Customer)
- description and source-code
```javascript
Customer = function (parameters) {
    this.ID = '';
    // These are named with camelCase because Dominos API uses this format
    if(!parameters){
        parameters={
            firstName:'',
            lastName:'',
            email:'',
            phone:''
        }
    }
    this.firstName = parameters.firstName;
    this.lastName = parameters.lastName;
    this.email = parameters.email;
    this.address = parameters.address;
    this.phone = parameters.phone;
}
```
- example usage
```shell
...

### creating an order

'''javascript

var pizzapi = require('dominos');

var thePresident = new pizzapi.Customer(
    {
        firstName: 'Barack',
        lastName: 'Obama',
        address: '700 Pennsylvania Avenue, Washington, DC',
        email: 'barack@whitehouse.gov'
    }
);
...
```

#### <a name="apidoc.element.dominos.Item"></a>[function <span class="apidocSignatureSpan">dominos.</span>Item (parameters)](#apidoc.element.dominos.Item)
- description and source-code
```javascript
Item = function (parameters) {
    if(!parameters){
        parameters={}
    }

    this.AutoRemove=false;

    this.Code = parameters.code||null;
    this.Qty = parameters.quantity||1;
    this.ID = 1;

    this.isNew = true;
    this.Options = { 'C': {'1/1': '1'}, 'X': {'1/1': '1'} };

    if(parameters.options) {
        for (var i=0; i<parameters.options.length; i++) {
            this.Options[parameters.options[i]] = { '1/1': '1' };
        }
    }
}
```
- example usage
```shell
...
'''

### Adding a product to the order :

'''javascript

order.addItem(
    new pizzapi.Item(
        {
            code: '14SCREEN',
            options: [],
            quantity: 1
        }
    )
);
...
```

#### <a name="apidoc.element.dominos.Menu"></a>[function <span class="apidocSignatureSpan">dominos.</span>Menu (menuData)](#apidoc.element.dominos.Menu)
- description and source-code
```javascript
Menu = function (menuData) {
    if(!menuData) {
        menuData={};
    } else {
        this.parseMenu(menuData);
    }
    this.menuData = menuData;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.MenuCategory"></a>[function <span class="apidocSignatureSpan">dominos.</span>MenuCategory (menuData, parentCategory)](#apidoc.element.dominos.MenuCategory)
- description and source-code
```javascript
MenuCategory = function (menuData, parentCategory) {
    if(!menuData) menuData={};

    this.menuData = menuData;
    this.subcategories = [];
    this.products = [];
    this.parent = parentCategory;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.MenuItem"></a>[function <span class="apidocSignatureSpan">dominos.</span>MenuItem (menuData)](#apidoc.element.dominos.MenuItem)
- description and source-code
```javascript
MenuItem = function (menuData) {
    if(!menuData) menuData={};

    this.menuData = menuData;
    this.categories = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.Order"></a>[function <span class="apidocSignatureSpan">dominos.</span>Order (parameters)](#apidoc.element.dominos.Order)
- description and source-code
```javascript
Order = function (parameters) {
  if(!parameters){
      parameters={}
  }
  //default order
  this.Address = '';
  this.Coupons = [];
  this.CustomerID = '';
  this.Email = '';
  this.Extension = '';
  this.FirstName = '';
  this.LastName = '';
  this.LanguageCode = 'en';
  this.OrderChannel = 'OLO';
  this.OrderID = '';
  this.OrderMethod = 'Web';
  this.OrderTaker = null;
  this.Payments = [];
  this.Phone = '';
  this.Products = [];
  this.Market = '';
  this.Currency = '';
  this.ServiceMethod = parameters.deliveryMethod || 'Delivery';
  this.SourceOrganizationURI = urls.sourceUri;
  this.StoreID = parameters.storeID||'';
  this.Tags = {};
  this.Version = '1.0';
  this.NoCombine = true;
  this.Partners = {};
  this.NewUser = true;
  this.metaData = {};
  this.Amounts = {};
  this.BusinessDate = '';
  this.EstimatedWaitMinutes = '';
  this.PriceOrderTime = '';
  this.AmountsBreakdown;

  if(parameters['customer']) {
    var Customer = parameters.customer;

    this.Address = Customer.address;
    this.CustomerID = Customer.ID;
    this.Email = Customer.email;
    this.FirstName = Customer.firstName;
    this.LastName = Customer.lastName;
    this.Phone = Customer.phone;
    return this;
  }
  if(parameters['Order'] || parameters['order']) {  //Used to initialize order object from Dominos results (Also handy for initializing
 from DB)
    var prevOrder = parameters.Order;
    var Customer = parameters.customer;

    this.Address = (Customer)? (
        (Customer.address)? Customer.address : prevOrder.Address
    ):prevOrder.Address;

    this.CustomerID = (Customer)? (
        (Customer.address)? Customer.ID : prevOrder.CustomerID
    ):prevOrder.CustomerID;

    this.Email = (Customer)? (
        (Customer.address)? Customer.email : prevOrder.Email
    ):prevOrder.Email;

    this.FirstName = (Customer)? (
        (Customer.address)? Customer.firstName : prevOrder.FirstName
    ):prevOrder.FirstName;

    this.LastName = (Customer)? (
        (Customer.address)? Customer.lastName : prevOrder.LastName
    ):prevOrder.LastName;

    this.OrderID = prevOrder.OrderID;
    this.Products = prevOrder.Products;
    this.Market = prevOrder.Market;
    this.Currency = prevOrder.Currency;
    this.StoreID = prevOrder.StoreID;
    this.Amounts = prevOrder.Amounts || {};
    this.BusinessDate = prevOrder.BusinessDate || '';
    this.EstimatedWaitMinutes = prevOrder.EstimatedWaitMinutes || '';
    this.PriceOrderTime = prevOrder.PriceOrderTime || '';
    this.AmountsBreakdown = prevOrder.AmountsBreakdown || {};

    return this;
  }
}
```
- example usage
```shell
...
firstName: 'Barack',
lastName: 'Obama',
address: '700 Pennsylvania Avenue, Washington, DC',
email: 'barack@whitehouse.gov'
      }
  );

  var order = new pizzapi.Order(
      {
customer: thePresident,

//optional set the store ID right away
storeID: myStore.ID,

deliveryMethod: 'Delivery' //(or 'Carryout')
...
```

#### <a name="apidoc.element.dominos.Store"></a>[function <span class="apidocSignatureSpan">dominos.</span>Store (parameters)](#apidoc.element.dominos.Store)
- description and source-code
```javascript
Store = function (parameters) {
    this.ID = parameters.ID;
}
```
- example usage
```shell
...
|--------|----|-------|--------|
|ID      |Integer|null|true    |

'''javascript

//Get Store Info for Store #4336
var pizzapi = require('dominos');
var myStore = new pizzapi.Store();
myStore.ID=4336;

myStore.getInfo(
    function(storeData){
        console.log(storeData);
    }
);
...
```



# <a name="apidoc.module.dominos.Menu"></a>[module dominos.Menu](#apidoc.module.dominos.Menu)

#### <a name="apidoc.element.dominos.Menu.Menu"></a>[function <span class="apidocSignatureSpan">dominos.</span>Menu (menuData)](#apidoc.element.dominos.Menu.Menu)
- description and source-code
```javascript
Menu = function (menuData) {
    if(!menuData) {
        menuData={};
    } else {
        this.parseMenu(menuData);
    }
    this.menuData = menuData;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dominos.Menu.prototype"></a>[module dominos.Menu.prototype](#apidoc.module.dominos.Menu.prototype)

#### <a name="apidoc.element.dominos.Menu.prototype.buildCategories"></a>[function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>buildCategories (categoryData, parent)](#apidoc.element.dominos.Menu.prototype.buildCategories)
- description and source-code
```javascript
buildCategories = function (categoryData, parent) {
    var category = new MenuCategory(categoryData,parent);
    for (var subIndex in categoryData.Categories) {
        category.getSubcategories().push(this.buildCategories(categoryData.Categories[subIndex],category));
    }
    categoryData.Products.forEach((function(productCode) { //link up products and categories
        var product = this.menuByCode[productCode];
        if (!product) {
            console.log("PRODUCT NOT FOUND: "+productCode,category.getCode());
            return;
        }
        category.getProducts().push(product);
        product.getCategories().push(category);
    }).bind(this));
    return category;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.Menu.prototype.getCouponCategory"></a>[function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>getCouponCategory ()](#apidoc.element.dominos.Menu.prototype.getCouponCategory)
- description and source-code
```javascript
getCouponCategory = function () {
    return this.rootCategories["Coupons"];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.Menu.prototype.getFoodCategory"></a>[function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>getFoodCategory ()](#apidoc.element.dominos.Menu.prototype.getFoodCategory)
- description and source-code
```javascript
getFoodCategory = function () {
    return this.rootCategories["Food"];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.Menu.prototype.getItemByCode"></a>[function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>getItemByCode (code)](#apidoc.element.dominos.Menu.prototype.getItemByCode)
- description and source-code
```javascript
getItemByCode = function (code) {
    return this.menuByCode[code];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.Menu.prototype.getPreconfiguredCategory"></a>[function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>getPreconfiguredCategory ()](#apidoc.element.dominos.Menu.prototype.getPreconfiguredCategory)
- description and source-code
```javascript
getPreconfiguredCategory = function () {
    return this.rootCategories["PreconfiguredProducts"];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.Menu.prototype.getRaw"></a>[function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>getRaw ()](#apidoc.element.dominos.Menu.prototype.getRaw)
- description and source-code
```javascript
getRaw = function () {
    return this.menuData;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.Menu.prototype.parseItems"></a>[function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>parseItems (parentMenuData, ParseClass)](#apidoc.element.dominos.Menu.prototype.parseItems)
- description and source-code
```javascript
parseItems = function (parentMenuData, ParseClass) {
    var items = [];
    Object.keys(parentMenuData).forEach((function(code) {
        var menuData = parentMenuData[code];
        var obj = new ParseClass(menuData);
        this.menuByCode[obj.getCode()] = obj;
        items.push(obj);
    }).bind(this));
    return items;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.Menu.prototype.parseMenu"></a>[function <span class="apidocSignatureSpan">dominos.Menu.prototype.</span>parseMenu (menuData)](#apidoc.element.dominos.Menu.prototype.parseMenu)
- description and source-code
```javascript
parseMenu = function (menuData) {
    this.menuByCode = {};
    var products = this.parseItems(menuData.result.Products,MenuItem);
    var coupons = this.parseItems(menuData.result.Coupons,MenuItem);
    var preconfigured = this.parseItems(menuData.result.PreconfiguredProducts,MenuItem);

    this.rootCategories = {}; //generate category tree using MenuCategory objects
    for (var categoryType in menuData.result.Categorization) {
        var categoryData = menuData.result.Categorization[categoryType];
        this.rootCategories[categoryType] = this.buildCategories(categoryData);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dominos.MenuCategory"></a>[module dominos.MenuCategory](#apidoc.module.dominos.MenuCategory)

#### <a name="apidoc.element.dominos.MenuCategory.MenuCategory"></a>[function <span class="apidocSignatureSpan">dominos.</span>MenuCategory (menuData, parentCategory)](#apidoc.element.dominos.MenuCategory.MenuCategory)
- description and source-code
```javascript
MenuCategory = function (menuData, parentCategory) {
    if(!menuData) menuData={};

    this.menuData = menuData;
    this.subcategories = [];
    this.products = [];
    this.parent = parentCategory;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dominos.MenuCategory.prototype"></a>[module dominos.MenuCategory.prototype](#apidoc.module.dominos.MenuCategory.prototype)

#### <a name="apidoc.element.dominos.MenuCategory.prototype.getCategoryPath"></a>[function <span class="apidocSignatureSpan">dominos.MenuCategory.prototype.</span>getCategoryPath ()](#apidoc.element.dominos.MenuCategory.prototype.getCategoryPath)
- description and source-code
```javascript
getCategoryPath = function () {
    var result = this.parent !== undefined ? this.parent.getCategoryPath().concat([this.menuData.Code]) : [this.menuData.Code];
    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.MenuCategory.prototype.getCode"></a>[function <span class="apidocSignatureSpan">dominos.MenuCategory.prototype.</span>getCode ()](#apidoc.element.dominos.MenuCategory.prototype.getCode)
- description and source-code
```javascript
getCode = function () {
    return this.menuData.Code;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.MenuCategory.prototype.getDescription"></a>[function <span class="apidocSignatureSpan">dominos.MenuCategory.prototype.</span>getDescription ()](#apidoc.element.dominos.MenuCategory.prototype.getDescription)
- description and source-code
```javascript
getDescription = function () {
    return this.menuData.Description;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.MenuCategory.prototype.getName"></a>[function <span class="apidocSignatureSpan">dominos.MenuCategory.prototype.</span>getName ()](#apidoc.element.dominos.MenuCategory.prototype.getName)
- description and source-code
```javascript
getName = function () {
    return this.menuData.Name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.MenuCategory.prototype.getProducts"></a>[function <span class="apidocSignatureSpan">dominos.MenuCategory.prototype.</span>getProducts ()](#apidoc.element.dominos.MenuCategory.prototype.getProducts)
- description and source-code
```javascript
getProducts = function () {
    return this.products;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.MenuCategory.prototype.getSubcategories"></a>[function <span class="apidocSignatureSpan">dominos.MenuCategory.prototype.</span>getSubcategories ()](#apidoc.element.dominos.MenuCategory.prototype.getSubcategories)
- description and source-code
```javascript
getSubcategories = function () {
    return this.subcategories;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dominos.MenuItem"></a>[module dominos.MenuItem](#apidoc.module.dominos.MenuItem)

#### <a name="apidoc.element.dominos.MenuItem.MenuItem"></a>[function <span class="apidocSignatureSpan">dominos.</span>MenuItem (menuData)](#apidoc.element.dominos.MenuItem.MenuItem)
- description and source-code
```javascript
MenuItem = function (menuData) {
    if(!menuData) menuData={};

    this.menuData = menuData;
    this.categories = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dominos.MenuItem.prototype"></a>[module dominos.MenuItem.prototype](#apidoc.module.dominos.MenuItem.prototype)

#### <a name="apidoc.element.dominos.MenuItem.prototype.getCategories"></a>[function <span class="apidocSignatureSpan">dominos.MenuItem.prototype.</span>getCategories ()](#apidoc.element.dominos.MenuItem.prototype.getCategories)
- description and source-code
```javascript
getCategories = function () {
    return this.categories;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.MenuItem.prototype.getCode"></a>[function <span class="apidocSignatureSpan">dominos.MenuItem.prototype.</span>getCode ()](#apidoc.element.dominos.MenuItem.prototype.getCode)
- description and source-code
```javascript
getCode = function () {
    return this.menuData.Code;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.MenuItem.prototype.getDescription"></a>[function <span class="apidocSignatureSpan">dominos.MenuItem.prototype.</span>getDescription ()](#apidoc.element.dominos.MenuItem.prototype.getDescription)
- description and source-code
```javascript
getDescription = function () {
    return this.menuData.Description;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.MenuItem.prototype.getName"></a>[function <span class="apidocSignatureSpan">dominos.MenuItem.prototype.</span>getName ()](#apidoc.element.dominos.MenuItem.prototype.getName)
- description and source-code
```javascript
getName = function () {
    return this.menuData.Name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.MenuItem.prototype.setCategories"></a>[function <span class="apidocSignatureSpan">dominos.MenuItem.prototype.</span>setCategories (categories)](#apidoc.element.dominos.MenuItem.prototype.setCategories)
- description and source-code
```javascript
setCategories = function (categories) {
    return this.categories = categories;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dominos.Order"></a>[module dominos.Order](#apidoc.module.dominos.Order)

#### <a name="apidoc.element.dominos.Order.Order"></a>[function <span class="apidocSignatureSpan">dominos.</span>Order (parameters)](#apidoc.element.dominos.Order.Order)
- description and source-code
```javascript
Order = function (parameters) {
  if(!parameters){
      parameters={}
  }
  //default order
  this.Address = '';
  this.Coupons = [];
  this.CustomerID = '';
  this.Email = '';
  this.Extension = '';
  this.FirstName = '';
  this.LastName = '';
  this.LanguageCode = 'en';
  this.OrderChannel = 'OLO';
  this.OrderID = '';
  this.OrderMethod = 'Web';
  this.OrderTaker = null;
  this.Payments = [];
  this.Phone = '';
  this.Products = [];
  this.Market = '';
  this.Currency = '';
  this.ServiceMethod = parameters.deliveryMethod || 'Delivery';
  this.SourceOrganizationURI = urls.sourceUri;
  this.StoreID = parameters.storeID||'';
  this.Tags = {};
  this.Version = '1.0';
  this.NoCombine = true;
  this.Partners = {};
  this.NewUser = true;
  this.metaData = {};
  this.Amounts = {};
  this.BusinessDate = '';
  this.EstimatedWaitMinutes = '';
  this.PriceOrderTime = '';
  this.AmountsBreakdown;

  if(parameters['customer']) {
    var Customer = parameters.customer;

    this.Address = Customer.address;
    this.CustomerID = Customer.ID;
    this.Email = Customer.email;
    this.FirstName = Customer.firstName;
    this.LastName = Customer.lastName;
    this.Phone = Customer.phone;
    return this;
  }
  if(parameters['Order'] || parameters['order']) {  //Used to initialize order object from Dominos results (Also handy for initializing
 from DB)
    var prevOrder = parameters.Order;
    var Customer = parameters.customer;

    this.Address = (Customer)? (
        (Customer.address)? Customer.address : prevOrder.Address
    ):prevOrder.Address;

    this.CustomerID = (Customer)? (
        (Customer.address)? Customer.ID : prevOrder.CustomerID
    ):prevOrder.CustomerID;

    this.Email = (Customer)? (
        (Customer.address)? Customer.email : prevOrder.Email
    ):prevOrder.Email;

    this.FirstName = (Customer)? (
        (Customer.address)? Customer.firstName : prevOrder.FirstName
    ):prevOrder.FirstName;

    this.LastName = (Customer)? (
        (Customer.address)? Customer.lastName : prevOrder.LastName
    ):prevOrder.LastName;

    this.OrderID = prevOrder.OrderID;
    this.Products = prevOrder.Products;
    this.Market = prevOrder.Market;
    this.Currency = prevOrder.Currency;
    this.StoreID = prevOrder.StoreID;
    this.Amounts = prevOrder.Amounts || {};
    this.BusinessDate = prevOrder.BusinessDate || '';
    this.EstimatedWaitMinutes = prevOrder.EstimatedWaitMinutes || '';
    this.PriceOrderTime = prevOrder.PriceOrderTime || '';
    this.AmountsBreakdown = prevOrder.AmountsBreakdown || {};

    return this;
  }
}
```
- example usage
```shell
...
firstName: 'Barack',
lastName: 'Obama',
address: '700 Pennsylvania Avenue, Washington, DC',
email: 'barack@whitehouse.gov'
      }
  );

  var order = new pizzapi.Order(
      {
customer: thePresident,

//optional set the store ID right away
storeID: myStore.ID,

deliveryMethod: 'Delivery' //(or 'Carryout')
...
```



# <a name="apidoc.module.dominos.Order.prototype"></a>[module dominos.Order.prototype](#apidoc.module.dominos.Order.prototype)

#### <a name="apidoc.element.dominos.Order.prototype.PaymentObject"></a>[function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>PaymentObject ()](#apidoc.element.dominos.Order.prototype.PaymentObject)
- description and source-code
```javascript
PaymentObject = function (){
    Object.defineProperties(
        this,
        {
            "Type": {
                writable:false,
                enumerable:true,
                value:"CreditCard"
            },
            "Amount":  {
                writable:true,
                enumerable:true,
                value:0
            },
            "Number":  {
                writable:true,
                enumerable:true,
                value:""
            },
            "CardType":  {
                writable:true,
                enumerable:true,
                value:""//uppercase
            },
            "Expiration":  {
                writable:true,
                enumerable:true,
                value:""//digits only
            },
            "SecurityCode":  {
                writable:true,
                enumerable:true,
                value:""
            },
            "PostalCode":  {
                writable:true,
                enumerable:true,
                value:""
            }
        }
    );
}
```
- example usage
```shell
...

'''javascript

var pizzapi = require('dominos');

var cardNumber = '4100123422343234';

var cardInfo = new order.PaymentObject();
cardInfo.Amount = order.Amounts.Customer;
cardInfo.Number = cardNumber;
cardInfo.CardType = order.validateCC(cardNumber);
cardInfo.Expiration = '0115';//  01/15 just the numbers "01/15".replace(/\D/g,'');
cardInfo.SecurityCode = '777';
cardInfo.PostalCode = '90210'; // Billing Zipcode
...
```

#### <a name="apidoc.element.dominos.Order.prototype.addCoupon"></a>[function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>addCoupon (Coupon)](#apidoc.element.dominos.Order.prototype.addCoupon)
- description and source-code
```javascript
addCoupon = function (Coupon) { //Add coupon to Order
    this.Coupons.push(Coupon)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.Order.prototype.addItem"></a>[function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>addItem (Item)](#apidoc.element.dominos.Order.prototype.addItem)
- description and source-code
```javascript
addItem = function (Item) { //Add product to Order
    this.Products.push(Item)
}
```
- example usage
```shell
...

'''

### Adding a product to the order :

'''javascript

order.addItem(
    new pizzapi.Item(
        {
            code: '14SCREEN',
            options: [],
            quantity: 1
        }
    )
...
```

#### <a name="apidoc.element.dominos.Order.prototype.mergeResponse"></a>[function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>mergeResponse (callback, response)](#apidoc.element.dominos.Order.prototype.mergeResponse)
- description and source-code
```javascript
mergeResponse = function (callback, response){
    for(var key in response.result.Order){
        if(util.isArray(response.result.Order[key])&&!response.result.Order[key].length){
            continue;
        }
        this[key]=response.result.Order[key];
    }
    //console.log(util.inspect(this.Products, { showHidden: true, depth: 5 }));
    if(callback){
        callback(response);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.Order.prototype.place"></a>[function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>place (callback)](#apidoc.element.dominos.Order.prototype.place)
- description and source-code
```javascript
place = function (callback) {
  if(!this.Products || !callback) {
      if(callback) {
          callback({
              success: false,
              message: 'At least one product must be added!'
          })
      }
  }

  var stringified = JSON.stringify({
    'Order' : this
  });

  httpJson.post(urls.order.place, stringified, callback);
}
```
- example usage
```shell
...
  cardInfo.CardType = order.validateCC(cardNumber);
  cardInfo.Expiration = '0115';//  01/15 just the numbers "01/15".replace(/\D/g,'');
  cardInfo.SecurityCode = '777';
  cardInfo.PostalCode = '90210'; // Billing Zipcode

  order.Payments.push(cardInfo);

  order.place(
      function(result) {
          console.log("Order placed!");
      }
  );

'''
...
```

#### <a name="apidoc.element.dominos.Order.prototype.price"></a>[function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>price (callback)](#apidoc.element.dominos.Order.prototype.price)
- description and source-code
```javascript
price = function (callback) {
  if(!this.Products || !callback) {
    if(callback) {
      callback({
        success: false,
        message: 'At least one Item must be added!'
      });
    }
    return;
  }

  var stringified = JSON.stringify({
    'Order' : this
  });

  httpJson.post(urls.order.price, stringified, this.mergeResponse.bind(this,callback));
}
```
- example usage
```shell
...

'''

### Price an Order

'''javascript

  order.price(
      function(result) {
          console.log("Price!")
      }
  );

'''
...
```

#### <a name="apidoc.element.dominos.Order.prototype.removeCoupon"></a>[function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>removeCoupon (Coupon)](#apidoc.element.dominos.Order.prototype.removeCoupon)
- description and source-code
```javascript
removeCoupon = function (Coupon) { //Remove coupon from Order
    var index = this.Coupons.indexOf(Coupon);
    if (index != -1) {
        this.Coupons.splice(index, 1);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.Order.prototype.removeItem"></a>[function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>removeItem (Item)](#apidoc.element.dominos.Order.prototype.removeItem)
- description and source-code
```javascript
removeItem = function (Item) {  //Remove product from Order
  var index = this.Products.indexOf(Item);
  if(index != -1) {
    this.Products.splice(index, 1);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dominos.Order.prototype.validate"></a>[function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>validate (callback)](#apidoc.element.dominos.Order.prototype.validate)
- description and source-code
```javascript
validate = function (callback) {  //Validate Order
  if(!this.Products || !callback) {
    if(callback) {
      callback({
        success: false,
        message: 'At least one Item must be added!'
      });
    }
    return;
  }

  //Blame Dominos, this isn't my doing.
  var stringified = JSON.stringify({
    'Order' : this
  });

  httpJson.post(urls.order.validate, stringified, this.mergeResponse.bind(this,callback));
}
```
- example usage
```shell
...
'''

### Validating an Order
This step is **Strongly** recommended

'''javascript

  order.validate(
      function(result) {
          console.log("We did it!");
      }
  );

'''
...
```

#### <a name="apidoc.element.dominos.Order.prototype.validateCC"></a>[function <span class="apidocSignatureSpan">dominos.Order.prototype.</span>validateCC (number)](#apidoc.element.dominos.Order.prototype.validateCC)
- description and source-code
```javascript
validateCC = function (number){
    var re = {
        visa        : /^4[0-9]{12}(?:[0-9]{3})?$/,
        mastercard  : /^5[1-5][0-9]{14}$/,
        amex        : /^3[47][0-9]{13}$/,
        diners      : /^3(?:0[0-5]|[68][0-9])[0-9]{11}$/,
        discover    : /^6(?:011|5[0-9]{2})[0-9]{12}$/,
        jcb         : /^(?:2131|1800|35\d{3})\d{11}$/,
        enroute     : /^(?:2014|2149)\d{11}$/
    };

    if (re.visa.test(number))
        return 'VISA';

    if (re.mastercard.test(number))
        return 'MASTERCARD';

    if (re.amex.test(number))
        return 'AMEX';

    if (re.diners.test(number))
        return 'DINERS';

    if (re.discover.test(number))
        return 'DISCOVER';

    if (re.jcb.test(number))
        return 'JCB';

    if (re.enroute.test(number))
        return 'JCB';

    return "";
}
```
- example usage
```shell
...
var pizzapi = require('dominos');

var cardNumber = '4100123422343234';

var cardInfo = new order.PaymentObject();
cardInfo.Amount = order.Amounts.Customer;
cardInfo.Number = cardNumber;
cardInfo.CardType = order.validateCC(cardNumber);
cardInfo.Expiration = '0115';//  01/15 just the numbers "01/15".replace(/\D/g,'');
cardInfo.SecurityCode = '777';
cardInfo.PostalCode = '90210'; // Billing Zipcode

order.Payments.push(cardInfo);

order.place(
...
```



# <a name="apidoc.module.dominos.Store"></a>[module dominos.Store](#apidoc.module.dominos.Store)

#### <a name="apidoc.element.dominos.Store.Store"></a>[function <span class="apidocSignatureSpan">dominos.</span>Store (parameters)](#apidoc.element.dominos.Store.Store)
- description and source-code
```javascript
Store = function (parameters) {
    this.ID = parameters.ID;
}
```
- example usage
```shell
...
|--------|----|-------|--------|
|ID      |Integer|null|true    |

'''javascript

//Get Store Info for Store #4336
var pizzapi = require('dominos');
var myStore = new pizzapi.Store();
myStore.ID=4336;

myStore.getInfo(
    function(storeData){
        console.log(storeData);
    }
);
...
```



# <a name="apidoc.module.dominos.Store.prototype"></a>[module dominos.Store.prototype](#apidoc.module.dominos.Store.prototype)

#### <a name="apidoc.element.dominos.Store.prototype.getFriendlyNames"></a>[function <span class="apidocSignatureSpan">dominos.Store.prototype.</span>getFriendlyNames (callback, lang)](#apidoc.element.dominos.Store.prototype.getFriendlyNames)
- description and source-code
```javascript
getFriendlyNames = function (callback, lang) {
  if( !this.ID || !callback){
      if(callback)
          callback({
              success: false,
              message: 'A callback is required to get a store menu'
          });
      return;
  }

  if(!lang)
      lang = 'en';

  var url = urls.store.menu.replace('${storeID}', this.ID)
      .replace('${lang}', lang);

  httpJson.get(url, function(result) {
    var itemMapping = [];
    var keys = Object.keys(result.result.Variants);
    keys.forEach(function(key) {
      var json = {};
      json[result.result.Variants[key].Name] = key
      itemMapping.push(json);
    });

    callback({ success: true, result: itemMapping });
  });
}
```
- example usage
```shell
...
'''javascript

  //Get friendly name menu for Store #4336
  var pizzapi = require('dominos');
  var myStore = new pizzapi.Store();
  myStore.ID = 4336;

  myStore.getFriendlyNames(
      function(storeData){
          console.log(storeData);
      }
  );

'''
...
```

#### <a name="apidoc.element.dominos.Store.prototype.getInfo"></a>[function <span class="apidocSignatureSpan">dominos.Store.prototype.</span>getInfo (callback)](#apidoc.element.dominos.Store.prototype.getInfo)
- description and source-code
```javascript
getInfo = function (callback) {
    if( !this.ID || !callback){
        if(callback)
            callback(
                {
                    success: false,
                    message: 'A callback is required to get store info'
                }
            );
        return;
    }

    httpJson.get(urls.store.info.replace('${storeID}', this.ID), callback);
}
```
- example usage
```shell
...
'''javascript

  //Get Store Info for Store #4336
  var pizzapi = require('dominos');
  var myStore = new pizzapi.Store();
  myStore.ID=4336;

  myStore.getInfo(
      function(storeData){
          console.log(storeData);
      }
  );

'''
...
```

#### <a name="apidoc.element.dominos.Store.prototype.getMenu"></a>[function <span class="apidocSignatureSpan">dominos.Store.prototype.</span>getMenu (callback, lang, noCache)](#apidoc.element.dominos.Store.prototype.getMenu)
- description and source-code
```javascript
getMenu = function (callback, lang, noCache) {
    if (this.cachedMenu && !noCache) {
        callback(this.cachedMenu); //TODO as below, break compatibility by removing first parameter
        return;
    }
    if( !this.ID || !callback){
        if(callback)
            callback({
                success: false,
                message: 'A callback is required to get a store menu'
            });
        return;
    }

    if(!lang)
        lang = 'en';

    var url = urls.store.menu.replace('${storeID}', this.ID)
        .replace('${lang}', lang);


    httpJson.get(url,(function(jsonObj) {
        this.cachedMenu = new Menu(jsonObj);
        callback(this.cachedMenu); //TODO break compatibility by removing first parameter
    }).bind(this));

<span class="apidocCodeCommentSpan">    /*
    httpJson.get(
        url,
        (function(response) {
            fs.writeFile('sampleResp/menu'+this.ID+'.json', JSON.stringify(response, null, 4), function (err) {
                if (err) throw err;
                console.log('It\'s saved!');
            });
        }).bind(this)
    );
    */
</span>}
```
- example usage
```shell
...
'''javascript

  //Get Menu for Store #4336
  var pizzapi = require('dominos');
  var myStore = new pizzapi.Store();
  myStore.ID = 4336;

  myStore.getMenu(
      function(storeData){
          console.log(storeData);
      }
  );

'''
...
```



# <a name="apidoc.module.dominos.Track"></a>[module dominos.Track](#apidoc.module.dominos.Track)

#### <a name="apidoc.element.dominos.Track.byId"></a>[function <span class="apidocSignatureSpan">dominos.Track.</span>byId (storeID, orderKey, callback)](#apidoc.element.dominos.Track.byId)
- description and source-code
```javascript
byId = function (storeID, orderKey, callback) {
    if(!storeID || !orderKey || !callback){
        if(callback)
            callback({
                success: false,
                message: 'storeID, orderKey, and callback are all required to get pizza info using the orderKey'
            });
        return;
    }

    this.byUrl(urls.track + 'StoreID=' + storeID + '&OrderKey=' + orderKey, callback);
}
```
- example usage
```shell
...
|storeID|sting or int|null|true|
|callback|function to pass the api result to|null|true|

'''javascript

var pizzapi = require('dominos');

pizzapi.Track.byId(
    123456,
    12345,
    function(pizzaData){
        console.log(pizzaData)
    }
);
...
```

#### <a name="apidoc.element.dominos.Track.byPhone"></a>[function <span class="apidocSignatureSpan">dominos.Track.</span>byPhone (phone, callback)](#apidoc.element.dominos.Track.byPhone)
- description and source-code
```javascript
byPhone = function (phone, callback) {
    if( !phone || !callback) {
        if(callback) {
            callback({
                success: false,
                message: 'Phone is required!'
            });
        }
        return;
    }

    this.byUrl(urls.track + 'Phone=' + phone, callback);
}
```
- example usage
```shell
...
|phone|Phone number string or int|null|true|
|callback|function to pass the api result to|null|true|

'''javascript

  var pizzapi = require('dominos');

  pizzapi.Track.byPhone(
      2024561111,
      function(pizzaData){
          console.log(pizzaData);
      }
  );

'''
...
```

#### <a name="apidoc.element.dominos.Track.byUrl"></a>[function <span class="apidocSignatureSpan">dominos.Track.</span>byUrl (url, callback)](#apidoc.element.dominos.Track.byUrl)
- description and source-code
```javascript
byUrl = function (url, callback){
    request.get(
        url,
        function (error, response, body) {
            if (error) {
                callback({
                    success: false,
                    message: error
                });
                return;
            }

            if (response.statusCode !== 200){
                callback({
                    success: false,
                    message:'HTML Status Code Error ' + response.statusCode
                });
                return;
            }

            var result = parser.toJson(
                body,
                {
                    coerce: false,
                    sanitize: false,
                    object: true,
                    trim: false
                }
            );

            if(!result['soap:Envelope']){
                callback({
                    success: false,
                    message: 'API soap:Envelope not present',
                    data: result
                });
                return;
            }

            if(!result['soap:Envelope']['soap:Body']){
                callback({
                    success: false,
                    message: 'API soap:Body not present',
                    data: result
                });
                return;
            }

            if(!result['soap:Envelope']['soap:Body'].GetTrackerDataResponse){
                callback({
                    success: false,
                    message:'API GetTrackerDataResponse not present',
                    data: result
                });
                return;
            }

            callback({
                orders: result['soap:Envelope']['soap:Body'].GetTrackerDataResponse.OrderStatuses,
                query: result['soap:Envelope']['soap:Body'].GetTrackerDataResponse.Query
            });
        }
    );
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dominos.Util"></a>[module dominos.Util](#apidoc.module.dominos.Util)

#### <a name="apidoc.element.dominos.Util.findNearbyStores"></a>[function <span class="apidocSignatureSpan">dominos.Util.</span>findNearbyStores (address, pickUpType, callback)](#apidoc.element.dominos.Util.findNearbyStores)
- description and source-code
```javascript
findNearbyStores = function (address, pickUpType, callback) {
    if(typeof pickUpType == 'function'){
        callback=pickUpType;
        pickUpType='Delivery';
    }
    if(!address || !callback) {
        if(!callback){
            throw('invalid findNearbyStores request. address and callback are required at a minimum.');
        }
        if(callback) {
            callback(
                {
                    success: false,
                    message: 'At least a partial address (minimum accepted is zipcode) is required to find stores'
                }
            );
        }
        return false;
    }

    var address = new Address(address)
    var addressLines=address.getAddressLines();

    var url = urls.store.find.replace(
        '${line1}',
        encodeURI(
          addressLines.line1
        )
    ).replace(
        '${line2}',
        encodeURI(
          addressLines.line2
        )
    ).replace(
        '${type}',
        pickUpType||'Delivery'
    );

    httpJson.get(url, callback);
}
```
- example usage
```shell
...
### By Postal Code
***this yields the least accurate information***

'''javascript

var pizzapi = require('dominos');

pizzapi.Util.findNearbyStores(
    '63102',
    'Delivery',
    function(storeData){
        console.log(storeData);
    }
);
...
```



# <a name="apidoc.module.dominos.http_json"></a>[module dominos.http_json](#apidoc.module.dominos.http_json)

#### <a name="apidoc.element.dominos.http_json.get"></a>[function <span class="apidocSignatureSpan">dominos.http_json.</span>get (url, callback)](#apidoc.element.dominos.http_json.get)
- description and source-code
```javascript
get = function (url, callback){
    var requestBody = {
        uri: url,
        headers: {
            'Referer': urls.referer
        }
    };
    http.get(requestBody, function (error, res, body) {
            if (error){  //If request errored out.
                callback({
                    success: false,
                    message: error
                });
                return;
            }
            if (res.statusCode !== 200){  //If request didn't error but response isn't status code 200.
                callback({
                    success: false,
                    message: 'HTML Status Code Error ' + res.statusCode
                });
                return;
            }

            try {
                var parsed = JSON.parse(body);
            }
            catch(error){
              console.log(error);
              return callback({
                  success: false,
                  message: error
              });
            }

            return callback({
                success: true,
                result: parsed
            });
        }
    );
}
```
- example usage
```shell
...
module.exports.get = function(url, callback){
var requestBody = {
    uri: url,
    headers: {
        'Referer': urls.referer
    }
};
http.get(requestBody, function (error, res, body) {
        if (error){  //If request errored out.
            callback({
                success: false,
                message: error
            });
            return;
        }
...
```

#### <a name="apidoc.element.dominos.http_json.post"></a>[function <span class="apidocSignatureSpan">dominos.http_json.</span>post (url, req, callback)](#apidoc.element.dominos.http_json.post)
- description and source-code
```javascript
post = function (url, req, callback) {
    if(typeof req !=  'string')
        req = JSON.stringify(req);

    var requestBody = {
        uri: url,
        headers: {
            Referer: urls.referer,
            'Content-Type': 'application/json'
        },
        body: req
    };
    http.post(requestBody, function (error, res, body) {
      if (error) {
          return callback({
            success: false,
            message: error
          });
      }

      if (res.statusCode !== 200) {
          return callback({
              success: false,
              message: 'HTML Status Code Error ' + res.statusCode
          });
      }

      try {
          var parsed = JSON.parse(body);
      }
      catch(error){
        console.log(error);
        return callback({
            success: false,
            message: error
        });
      }

      return callback({
          success: true,
          result: parsed
      });
  });
}
```
- example usage
```shell
...
    uri: url,
    headers: {
        Referer: urls.referer,
        'Content-Type': 'application/json'
    },
    body: req
};
http.post(requestBody, function (error, res, body) {
  if (error) {
      return callback({
        success: false,
        message: error
      });
  }
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
