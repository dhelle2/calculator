#include <stack>
#include <iostream>

using namespace std;

int main() {
  stack<int> st;

  char in;

  int total;

  while(in != 'q') {
    cin >> in;
    if(isdigit(in)) st.push(in-'0');
    else if(in == 'q') continue;
    else {
     int digit = st.top();
     st.pop(); 
     switch(in) {
      case '+':
       total = total + digit;
       break;
      case '-':
       total = total - digit;
       break;
      case '*':
       total = total * digit;
       break;
      case '/':
       total = total / digit;
       break;
      case '%':
       total = total % digit;
       break;
      default:
       cout << "operator unrecognized ... last digit discarded.." << endl;
     }// switch
     cout << total << endl;
    }// else
  }

}
