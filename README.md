Code segment: aby

Inheritance Patterns used: Inheritance

Design Patterns used: Prototype

Usage justification: The Script needs a new storebranch with the same data as an existing storebranch. 
Using a clone of NewYrokBranch and changing only whats necessary into a seperate object. 
this shallow copy allows for 
Los Angeles to be changed without NewYork being changed.


Code segment: cwm

Inheritance Patterns used: Abstraction

Design Patterns used: Factory

Usage justification: Object Creation is abstracted out to its subclasses using the factory method BuildAuthorization.
The website has signinauthentication and cart returns signupauthentication, and the base class treats both as IAuthentication.
new authentication methods can be added without changing more code.


Code segment: kef

Inheritance Patterns used: Interface 

Design Patterns used: Proxy

Usage justification: Defining IMoney with Buy means all payment can be used the same way. code that spends money does not require and particular class of payment.
The script only has credit card but shows foundation.


Code segment: kir

Inheritance Patterns used:  Interface

Design Patterns used:Proxy

Usage justification: OnlinePayment holds an IMoney reference and sends MakeAPurchase to Money.Buy. The caller buys through Online Payment rather than interacting with the Credit Card Directly, so OnlinePayment only adds checks and extra steps around the request reaches the real payment object and finishes the transation.Because it only needs the IMoney interface, other payment types could replace the old ones without major changes.


Code segment: pyx

Inheritance Patterns used: Interface

Design Patterns used: Adapter

Usage justification:  ImammothBank needs a Pay method, but EtherPayment only has TransactEther. Adapter Translates the two so that the existing class is not modified.
EtherAdapter Intakes Pay() and then processes it into TransactEther() to execute this filter from one into the other in a isolated enviornemnt.


Code segment: ret

Inheritance Patterns used: standard Inheritance

Design Patterns used: singleton

Usage justification: Person has a Private Static Instance and exposes it through a public static instance that creates the object only once.
In Main, person 1 and 0 are the same object.
When one shared object is needed this reference becomes useful as a isolated unit.


Code segment: rom

Inheritance Patterns used: Standard Inheritance 

Design Patterns used: Adapter

Usage justification: EtherPayment has its own Transact method and shares no interface with the rest of the script. It has the problem that the adapter solves of filtering from one method to another and keeping who methods separate with a new script.


Code segment: tow

Inheritance Patterns used: Abstraction

Design Patterns used: Factory

Usage justification: The scripts declare an abstract factory, and website is meant to supply the concrete product. It receives a subclass with a IAuthorization then builds the specific kind that it needs. Creating new authentications in pair with adaption.


Code segment: vug

Inheritance Patterns used:  Interface

Design Patterns used: Adapter

Usage justification: 
The complete setup has the IMammothBank.Pay all on the clientside. Ether Adapater translates that call into EtherPayment.TransactEther(). The store  can accept Ether payments without changing Store or EtherPayment. 
Other Payment systems could be added to this to process other types.
