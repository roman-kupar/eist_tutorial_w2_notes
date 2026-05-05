# Notes W02
Tutorial notes for System Design I Modularity and Data Management

## Modules
<img width="1000" height="550" alt="image" src="https://github.com/user-attachments/assets/2600cea1-1fd3-44c1-aab1-073a2470e405" />

---

- The best modules are deep (powerful functionality with a simple interface). 
- The actual implementation should be almost always abstracted away in a simple interface for external usage
- Achieve low coupling and high cohesion

## Facade 

<img width="380" height="272" alt="image" src="https://github.com/user-attachments/assets/20ddc16c-f30b-417e-82cc-4632fc804d5a" />

---

- Unifies interaction with module components in one single interface, easy to use
- Also easier for a client, to communicate through a facade, and not through different microservices.

## Layered Architecture
<img width="791" height="496" alt="image" src="https://github.com/user-attachments/assets/5cfe48a0-cc8d-4089-85f4-8bdb56d36cba" />

---

- Split software into layers, where each layer can only refer to a layer below, not a layer above
- Open: a layer can refer to any layer below
- Closed: a layer can only refer to a layer (n-1) below

## Data Management

<img width="804" height="622" alt="image" src="https://github.com/user-attachments/assets/39982baa-73ef-4b5e-b931-c8219a59938d" />

<img width="662" height="487" alt="image" src="https://github.com/user-attachments/assets/4af06352-d8dd-4f59-a84e-86ae65e4876d" />

<img width="612" height="407" alt="image" src="https://github.com/user-attachments/assets/a47feb15-6b06-4252-8ea6-4433930a095b" />

## MVC

<img width="816" height="456" alt="image" src="https://github.com/user-attachments/assets/937f90e3-86c2-472d-8174-3b50690cfae5" />

Model-view-controller

- A specific pattern, in which software code orchestrates.
- Model: defines the main objects, on which Controller and View part operate
- View: handles the updates on the view for client to see.
- Controller: handles the bussiness logic.
- Each part doesn't invervene with each other, and only "notifies", when some action is required.
