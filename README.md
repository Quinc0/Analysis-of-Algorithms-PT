# Data Structures in C++

This repository provides implementations of various data structures in C++ including Circular Linked Lists, Singly Linked Lists, Doubly Linked Lists, Queues, Heaps, Trees, Graphs, and Stacks. Below are the descriptions and code snippets for each data structure.

## Circular Linked Lists

A circular linked list is a linked list where the last node points back to the first node.

```cpp
#include <iostream>

struct Node {
    int data;
    Node* next;
};

class CircularLinkedList {
public:
    CircularLinkedList() : head(nullptr) {}

    void insert(int data) {
        Node* newNode = new Node{data, head};
        if (!head) {
            head = newNode;
            head->next = head;
        } else {
            Node* temp = head;
            while (temp->next != head) {
                temp = temp->next;
            }
            temp->next = newNode;
            newNode->next = head;
        }
    }

    void printList() {
        if (!head) return;
        Node* temp = head;
        do {
            std::cout << temp->data << " -> ";
            temp = temp->next;
        } while (temp != head);
        std::cout << "HEAD\n";
    }

private:
    Node* head;
};

int main() {
    CircularLinkedList list;
    list.insert(1);
    list.insert(2);
    list.insert(3);
    list.printList();
    return 0;
}
