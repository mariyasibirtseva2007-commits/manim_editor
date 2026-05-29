from manim import *

class Hello(Scene):
    def construct(self):

        text = Text("HELLO")

        self.play(Write(text))

        self.wait(1)

        self.play(text.animate.scale(2))

        self.play(
            text.animate.shift(UP * 2)
        )

        square = Square()

        self.play(Create(square))

        self.play(
            square.animate.rotate(PI)
        )

        self.wait(2)
