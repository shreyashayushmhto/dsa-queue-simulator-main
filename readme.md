🚦 Real-Time Traffic Queue Simulation
Hey there! This project is a real-time traffic simulation that showcases how queue data structures can be used for traffic management. It includes different types of vehicles, traffic lights, and priority-based queuing to make traffic flow smooth and realistic.



✨ What's Inside?
🏎️ 4-way intersection simulation in real-time
🚓🚑🚒 Different vehicle types with priority handling (like ambulances and fire trucks)
🚦 Traffic light system that dynamically changes
🔄 Vehicles can turn left, right, or go straight
🎯 Queue-based traffic management for smoother flow
⚙️ What You Need
To run this project, you'll need:

🖥️ GCC/G++ compiler (for compiling the code)
🎮 SDL2 library (for graphics and rendering)
🏗️ MinGW (for Windows users)
🛠 How to Install SDL2?
If you're using Windows:
🔗 Download SDL2
📂 Extract the files to your project folder
🏗 Create these folders if they don’t exist:
include/ → for header files
lib/ → for library files
bin/ → for the executable output
📂 Project Folder Structure
Your project will be organized like this:

makefile
Copy
Edit
DSA-Queue-Simulator/
├── include/          # Header files  
├── lib/              # Library files  
├── src/              # Source code  
├── bin/              # Executable files  
└── README.md         # This file!  
🚀 Ready to Run?
Compile and run the project with this command:


g++ -Iinclude -Llib -o bin/main.exe src/main.c src/traffic_simulation.c -lmingw32 -lSDL2main -lSDL2
And that’s it! 🎉 Now you can see the traffic simulation in action. 🚦🚗💨






Traffic Queue Simulator
A real-time traffic simulation implementing queue-based traffic management. The system models a 4-way intersection, incorporating multiple vehicle types, traffic lights, and priority-based queuing.

Features
Real-time simulation of a 4-way intersection
Support for multiple vehicle types with priority handling
Dynamic traffic light system
Vehicles can turn left, right, or proceed straight
Queue-based traffic management for efficient flow control
Prerequisites
To build and run the project, ensure you have the following:

GCC/G++ compiler
SDL2 library
MinGW (for Windows users)
Installing SDL2
For Windows Users:
Download SDL2 from the official website.
Extract the contents into the project directory.
Ensure the following folders exist:
include/ (for header files)
lib/ (for library files)
bin/ (for executable output)
Project Structure

DSA-Queue-Simulator/
├── include/          # Header files  
├── lib/              # Library files  
├── src/              # Source files  
├── bin/              # Executables  
└── README.md  
Building the Project
Clone the repository:

bash
git clone:https://github.com/shreyashayushmhto/dsa-queue-simulator-main
cd DSA-Queue-Simulator  
Compile the project:

g++ -Iinclude -Llib -o bin/main.exe src/main.c src/traffic_simulation.c -lmingw32 -lSDL2main -lSDL2  
bash

g++ -o bin/generator src/generator.c src/traffic_simulation.c -lSDL2 -Iinclude -Llib -lmingw32 -lSDL2main -lSDL2  
Running the Simulation
Start the vehicle generator:

./bin/generator  
In another terminal, run the main simulation:

bash
./bin/main  
Observe vehicle movements at the intersection.

Close the simulation by clicking the exit button.

Vehicle Types
Regular cars
Ambulances
Police cars
Fire trucks
Traffic Management
Queue System: Each lane maintains a queue of vehicles.
Priority Handling: Emergency vehicles receive priority access.
Traffic Light Cycles: Red and green light transitions occur automatically.
Turn Management: Vehicles follow predefined movement rules for left, right, and straight directions.
Code Highlights
Queue Data Structure
c
Copy
Edit
typedef struct Node {
    Vehicle vehicle;
    struct Node* next;
} Node;

typedef struct {
    Node* front;
    Node* rear;
    int size;
} Queue;
Vehicle States
c
Copy
Edit
typedef enum {
    STATE_MOVING,
    STATE_STOPPING,
    STATE_STOPPED,
    STATE_TURNING
} VehicleState;
Contributing
Fork the repository.
Create a new branch:
bash
Copy
Edit
git checkout -b feature/your-feature  
Commit changes:
bash
Copy
Edit
git commit -m "Describe your changes"  
Push to the branch:
bash
Copy
Edit
git push origin feature/your-feature  
Open a pull request.
References
SDL2 Documentation
CLRS: Queue Data Structures
Highway Capacity Manual (Traffic Flow Theory)
Acknowledgments
SDL2 Development Team
Researchers in Traffic Simulation
Contributors and Testers
