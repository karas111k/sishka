#include "list.h"
#include <iostream>
#include <string>
using namespace std;

void list::print()
{
  if (empty()) return;
  element* p = head;
  int counter = 0;
  cout << "№\t" << "value\t" << "p\t\t" << "prev\t\t" << "next" << endl;
  while (p) {
    cout << counter << "\t" << p->value << "\t" << p << "\t" << p->prev << "\t" << p->next << endl;
    p = p->next;
    counter++;
  }
}

void element::print()
{
  cout << value << endl;
}


bool list::empty()
{
  return head == nullptr;
}

element::element(const element& other)
{
  value = other.value;
  next = other.next;
  prev = other.prev;
}

element::element(double v)
{
  value = v;
  next = nullptr;
  prev = nullptr;
}

list::list()
{
  head = nullptr;
  tail = nullptr;
}

void list::push_back(const element& elem)
{
  element* p = new element(elem);
  size++;
  
  if (empty()) {
    head = p;
    tail = p;
    return;
  }
  tail->next = p;
  p->prev = tail;
  tail = p;
}
void list::push_front(const element& elem)
{
  element* p = new element(elem);
  size++;
  
  if (empty()) {
    head = p;
    tail = p;
    return;
  }
  head->prev = p;
  p->next = head;
  head = p;
}

// int main () {
//   element Node(5);
//   Node.print();
  int main (){
  list List;
//   List.push_back(1);
//   List.push_back(2);
//   List.push_back(3);
//   List.push_front(0);
//   List.pop_front();
//   List.pop_back();
  
  List.print();
  
  
  return 0;
}
