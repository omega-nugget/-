import turtle

t = turtle.Turtle()
t.shape('turtle')

# Функция для рисования яруса с заданным цветом
def рисовка (width, height, color):
    t.begin_fill()
    t.fillcolor(color)
    for _ in range(2):
        t.fd(width)
        t.lt(90)
        t.fd(height)
        t.lt(90)
    t.end_fill()
    
t.up()
t.goto(-200, -150)
t.down()

# нижний ярус
рисовка(400, 100, 'pink')

# _______________________
t.up()
t.goto(-150, -50)
t.down()


рисовка(300, 80, 'pink')

# _____________________
t.up()
t.goto(-100, 30)
t.down()


рисовка(200, 60, 'pink')

# свечи-1
t.up()
t.goto(-50, 90)
t.down()
t.color('green')
t.lt(90)
t.fd(90)
t.circle(9)

t.color('red')
t.begin_fill()
t.circle(9)
t.end_fill()

# Свечи 2
t.up()
t.goto(0, 90)
t.down()
t.color('blue')
t.fd(90)
t.circle(9)

t.color('red')
t.begin_fill()
t.circle(9)
t.end_fill()

# Свеча 3
t.up()
t.goto(50, 90)
t.down()
t.color('violet')
t.fd(90)
t.circle(9)

t.color('red')
t.begin_fill()
t.circle(9)
t.end_fill()
