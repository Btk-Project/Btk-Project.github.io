# Welcome to BtkProject Homepage

Btk is a gui tookit written in C++17  

## Example

This a example how to create a window  

```cpp
//Include all headers
#include <Btk.hpp>
int main(){
    //Do init
    Btk::Init(); 
    //Create a window
    Btk::Window win("Hello World",100,100);
    //Add a button
    auto &btn = win.add<Btk::Button>();
    //Set text
    btn.set_text("Close the window");
    //Connect signal
    btn.sig_click().connect([&win]{
        win.close();
    });
    //Enter the eventloop
    return win.mainloop();
}

```

For more details see in [GitHub](https://github.com/BusyStudent/Btk)

## Support  

Fork and send PR
