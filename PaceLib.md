[Back](https://greengolem.github.io)
<hr>
<br>
## Pace Lib

2d c++ graphics library (based on SDL2).

Focus on easy to use API.

Flexible widget system (json configuration or code).

Designed for 2d games (focus on point and click)

Good documentation

### Usage

Check the available examples:
blank, main_menu, graphics, gui, point_and_click, sdl2

After the initialization:

    Text::Create("title_txt");
    Button::Create("new_btn");
    Button::Create("options_btn");
    Button::Create("help_btn");
    Button::Create("exit_btn");

In the wconfs folder the corresponding configurations:

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

    etc

The other option is to just use code.

### Code

### Buy

Open source version:

&nbsp;&nbsp;&nbsp;&nbsp;[PaceLib on github](https://github.com/aiafrasinei/PaceLib)

### Manual

&nbsp;&nbsp;&nbsp;&nbsp;[Code documention](https://greengolem.github.io/PaceLib/html/index.html)
