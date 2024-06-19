#include <iostream>
#include <string>

// Define a class for a tranquil grove
class TranquilGrove {
private:
    std::string name;
    int treeCount;
    bool hasStream;

public:
    // Constructor
    TranquilGrove(const std::string& name, int treeCount, bool hasStream) 
        : name(name), treeCount(treeCount), hasStream(hasStream) {}

    // Method to display information about the grove
    void displayInfo() {
        std::cout << "Welcome to " << name << " tranquil grove.\n";
        std::cout << "There are " << treeCount << " trees here.\n";
        if (hasStream) {
            std::cout << "There is a peaceful stream flowing through the grove.\n";
        } else {
            std::cout << "This grove is calm and serene.\n";
        }
    }

    // Method to simulate a day passing in the grove
    void simulateDay() {
        std::cout << "The sun rises over the " << name << " grove.\n";
        if (hasStream) {
            std::cout << "Birds chirp near the stream.\n";
        } else {
            std::cout << "A gentle breeze rustles through the trees.\n";
        }
        std::cout << "The day passes peacefully in the grove.\n";
    }
};

int main() {
    // Create an instance of TranquilGrove
    TranquilGrove myGrove("Tranquil Grove", 50, true);

    // Display information about the grove
    myGrove.displayInfo();

    // Simulate a day passing in the grove
    myGrove.simulateDay();

    return 0;
}
