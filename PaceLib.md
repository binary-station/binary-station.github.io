[Back](https://binary-station.github.io)
<hr>
<br>
## Pace Lib

Open source 2d c++ graphics library (based on SDL2).

Easy to use

Flexible widget system (json configuration or code).

Designed for 2d games

Examples

Good documentation

### Prerequisites

&nbsp;&nbsp;&nbsp;&nbsp;Linux/Windows/MacOs

&nbsp;&nbsp;&nbsp;&nbsp;c++20 compiler

&nbsp;&nbsp;&nbsp;&nbsp;SDL2 for rendering

&nbsp;&nbsp;&nbsp;&nbsp;SDL2_image

&nbsp;&nbsp;&nbsp;&nbsp;SDL2_ttf 

&nbsp;&nbsp;&nbsp;&nbsp;cmake

### Usage

&nbsp;&nbsp;&nbsp;&nbsp;[Examples](https://github.com/aiafrasinei/PaceLib/tree/main/examples)

&nbsp;&nbsp;&nbsp;&nbsp;Check the available examples:

&nbsp;&nbsp;&nbsp;&nbsp;blank, main_menu, graphics, gui, tictactoe, sdl2

&nbsp;&nbsp;&nbsp;&nbsp;After the PaceLib initialization:

    Text::Create("title_txt");
    Button::Create("new_btn");
    
&nbsp;&nbsp;&nbsp;&nbsp;In the wconfs folder the corresponding json configurations:

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

&nbsp;&nbsp;&nbsp;&nbsp;Widgets can have child elements example:

    Tab::BeginBlock("second_tab");
        Text::Begin("text");
	 Label::BeginBlock("out_lbl");
             DefaultTooltip::Begin("out_tooltip");
	 Label::EndBlock();
	 TextArea::Begin("text_ta");
	 TextInput::Begin("tinput");
	 CheckBox::Begin("cb");
    Tab::EndBlock();

&nbsp;&nbsp;&nbsp;&nbsp;Event handling:

    Tab::BeginBlock("first_tab");
        Label::Begin("label_lbl");
	Button::Begin("start_btn");
	Button::Begin("exit_btn");
    Tab::EndBlock();
			
    root->GetTab("first_tab")->GetButton("exit_btn")->onClickCallback = []() {
         Window::running = false;
    };
	   
&nbsp;&nbsp;&nbsp;&nbsp;The other option is to use the programatic api:

    Text::Begin({root, "text"},
        {root->GetScene("Default")->GetFont("lazy_font"), "some text"},
        600, 100, {50, 50, 50, 255});

### Screenshots

| gui | tictactoe |
| --- | --- |
| [image](images/s1_PaceLib.jpg) | [image](images/s2_PaceLib.png) |

### Get

&nbsp;&nbsp;&nbsp;&nbsp;[PaceLib on github](https://github.com/aiafrasinei/PaceLib)

### Manual

&nbsp;&nbsp;&nbsp;&nbsp;[Code documention](https://binary-station.github.io/PaceLib/html/index.html)
