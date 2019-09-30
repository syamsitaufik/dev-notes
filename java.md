oop
- encapsulation
  - protect / hide / control access of variable
  - provide methods to access or modify value
  
- inheritance
  - a class which can acquire properties & functionalities from another class
  - parent-child or super-sub relationship
  - single = class
  - multi = interfaces
  - multi-level = a class/interface that extends another class/interface that extends another class/interface and so on
  - hierarchical = multiple class/interface extends same class/interface

- polymorphism
  - same actions/functionalities with different forms
  - static = overload = members
  - dynamic = overrride = inheritance
  
- abstraction
  - inheritance with partial implementation in super/parent class.
  - it will be done, non optional, by the sub/child classes

heap = instances and runtime string/constant
 - xms = start
 - xmx = max
stack = methods, primitives, reference
 - xss = size

garbage collection
- daemon thread, watch unused objects in heap, then destroy
- mark & sweep
- young generation = newly created and short lifetime
  - eden = new
  - survivor = not cleared from eden first collect
- old generation = movedn from young because of longer lifetime
- permanent = method, string, constant
- method for old gen
  - serial = mark-sweep-compact
    - single thread
    - small heap and less cpu
    
  - parallel = 
    - multi thread
    - big heap and more cpu
    
  - parallel old = old gen only
  
  - concurrent = low latency
    - shorter STW pause but frequent
    - very high cpu
    - too much fragments -> compact -> longer STW pause
    
  - G1
    - split heap into regions (2mb each)
    - collect only if full or almost full

rest = representational state transfer
 - uniform =  1 uri for a resource (identification,manipulation,self-descriptive, hateoas)
 - client-server = no dependency, can be added/removed/replaced anytime
 - stateless = no session, no history
 - cacheable = faster
 - layered = intermediary/proxy
 - code on demand = return code if needed instead of actual data/payload
