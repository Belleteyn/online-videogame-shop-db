# online-videogame-shop-db
A model of a database for an online shop selling video games. Made in MySQL Workbench. Only necessary entities and attributes are included.

The main entities are Game and OrderHeader. OrderHeader represents a single order. OrderDetail represents a single item in the order.
For an order to be made, there are a few things needed: customer data, payment method, order status, delivery method and possibly delivery address.
These entities were made because this data can and should be reused. 

DeliveryAddress and Customer reuse Address. Delivery address can be different from Customer's billing address. 
DeliveryAddress may also not exist at all, for example when self-pickup is chosen.

A game is often made for many platforms but fundamentally that is still the same game. PEGI is required. Games are usually available in more than one language.
Translations may include subtitles or dubbing (language version type).

A game can belong to many genres. 
