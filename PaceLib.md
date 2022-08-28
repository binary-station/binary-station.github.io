[Back](https://binary-station.github.io)
<hr>
<br>
## Pace Lib

Open source 2d c++ graphics library (based on SDL2).

Easy to use

Flexible widget system (json configuration or code).

Designed for 2d games

[Examples](https://github.com/aiafrasinei/PaceLib/tree/main/examples)

[Code documentation](https://binary-station.github.io/PaceLib/html/index.html)

### Prerequisites

Linux/Windows/MacOs

c++20 compiler

SDL2 for rendering

SDL2_image

SDL2_ttf 

cmake

### Usage

Check the available examples:

blank, main_menu, graphics, gui, tictactoe, sdl2

After the PaceLib initialization:

    Text::Create("title_txt");
    Button::Create("new_btn");
    
In the wconfs folder the corresponding json configurations:

    title_txt.wconf:

    {
        "scene" : "Default",
        "font" : "font_title",
        "text" : "Game",
        "pos" : ["W_2%", "H_1%"],
        "text_color" : [140, 190, 140, 255]
    }

    new_btn.wconf:

    {
        "dim" : ["W_2%", "H_10%", "W_7.5%", "H_3%"],
        "color" : [40, 40, 40, 255],
        "scene" : "Default",
        "font" : "default",
        "text" : "New",
        "text_color" : [140, 170, 140, 255],
        "align" : ["mid", "mid"]
    }

Widgets can have child elements example:

    Tab::BeginBlock("second_tab");
		Text::Begin("text");
		Label::BeginBlock("out_lbl");
			DefaultTooltip::Begin("out_tooltip");
		Label::EndBlock();
		TextArea::Begin("text_ta");
		TextInput::Begin("tinput");
		CheckBox::Begin("cb");
	Tab::EndBlock();
    
Event handling:

    Tab::BeginBlock("first_tab");
		Label::Begin("label_lbl");
		Button::Begin("start_btn");
		Button::Begin("exit_btn");
	Tab::EndBlock();
	
	root->GetTab("first_tab")->GetButton("exit_btn")->onClickCallback = []() {
		Window::running = false;
    };
   
The other option is to use code.

### Get

Open source version:

&nbsp;&nbsp;&nbsp;&nbsp;[PaceLib on github](https://github.com/aiafrasinei/PaceLib)

### Manual

&nbsp;&nbsp;&nbsp;&nbsp;[Code documention](https://binary-station.github.io/PaceLib/html/index.html)
