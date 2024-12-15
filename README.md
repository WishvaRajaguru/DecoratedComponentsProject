# 🎨 About DecoratedComponentsProject
    
The DecoratedComponentsProject is a lightweight Java Swing library designed to simplify the creation of visually appealing UI components. The library currently provides two powerful components:

- DecoratedPanel
- DecoratedImagePanel

This library is a perfect choice for developers looking to enrich their Swing applications with enhanced visuals without compromising performance.

<hr/>
<br/>
<br/>
<br/>

## ✨ Features

⁜ IDE drag & drop designing support (Netbeans).
<br/>
⁜ Easily understandable property customization.

🖼️ <b> DecoratedPanel </b>

- Customizable rouded corners and background colors.

🌄 <b> DecoratedImagePanel </b>

- Display images seamlessly with advanced scaling options.
- Smooth rendering for high-resolution images.
<br/>
<br/>

## 🚀 Getting Started

Installation

Simply download the  <i>.jar</i> file and Add the library to your project.
<br/>
<br/>

## Usage

The usage is pretty self explanatory since it is easy with Netbeans IDE. (Explained usage instructions will be added sooner!)
<br/>

### DecoratedPanel

- Create a new DecoratedPanel Object and set border radius as needed:

```java
    import com.rajaguru.DecoratedPanel;
    import javax.swing.*;

    public class Main {
        public static void main(String[] args) {
            JFrame frame = new JFrame("DecoratedPanel Example");
            DecoratedPanel panel = new DecoratedPanel();
            panel.setBackgroundColor(Color.BLUE);

            //To set Top-Left Radius
            panel.setArchTopLeft(100);

            //To set Top-Right Radius
            panel.setArchTopRight(100);

            //To set Bottom-Right Radius
            panel.setArchBottomRight(100);

            //To set Bottom-Left Radius
            panel.setArchBottomLeft(100);
    
            frame.add(panel);
            frame.setSize(800, 800);
            frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
            frame.setVisible(true);
        }
    }
```

<br/>

### DecoratedImagePanel

- Create a new DecoratedImagePanel Object and set the Image:

```java
    import com.rajaguru.DecoratedImagePanel;
    import javax.swing.*;
    import javax.swing.ImageIcon;
    
    public class Main {
        public static void main(String[] args) {
            JFrame frame = new JFrame("DecoratedPanel Example");
            DecoratedImagePanel panel = new DecoratedImagePanel();

            //Add Image to panel
            panel.setImageIcon(new ImageIcon(getClass().getResource("path")));
    
            frame.add(panel);
            frame.setSize(800, 800);
            frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
            frame.setVisible(true);
        }
    }
```

- Set the border radius for DecoratedImagePanel:

```java
            //MAKE SURE TO SET THIS PROPERTY TRUE TO ACTIVATE THIS FEATURE
            panel.setRoundedCorners(true);

            //To set Top-Left Radius
            panel.setArchTopLeft(100);

            //To set Top-Right Radius
            panel.setArchTopRight(100);

            //To set Bottom-Right Radius
            panel.setArchBottomRight(100);

            //To set Bottom-Left Radius
            panel.setArchBottomLeft(100);
```

- To center image within the panel:

```java
            panel.setCenterImage(true);
```

- To Fit the image to the container:

```java
            panel.setFitContent(true);
```

- To Enable Smooth Rendering of the image:
This feature may slow down the loading process based on the performance of your workstation. How ever this will get rid of that laggy edges of the image if you need it.

```java
            panel.setSmoothDecoration(true);
```
<br/>
<br/>

## 🛠️ Built With

- Java Swing
- JDK 8+
<br/>

## 🧑‍💻 Author

- Wishva Rajaguru @ wishvarajaguru@gmail.com
<br/>
Connect with me on <a href=""> GitHub </a>!
<br/>

## 📜 License

This project is licensed under the MIT License. See the <a href='LICENSE'>LICENSE </a> file for details.
<br/>

## 🙌 Support

If you find this project helpful, please ⭐ the repository and share it with others!
