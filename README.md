# iQuHACK-quantum-cat
#iQuHACK quantum computing video game


import pygame

#initialize pygame
pygame.init()

#setting up screen dimensions
screen = pygame.display.set_mode((1220,800))

#Window name and Icon
pygame.display.set_caption("Quantum Cat")
icon = pygame.image.load('cat0.png')
pygame.display.set_icon(icon)

#Title
font = pygame.font.Font('freesansbold.ttf',32)
BLACK = (0,0,0)
img = font.render('Try to Find:', True, BLACK)

#background
background = pygame.image.load('start.png')

#Cats
cat0Img = pygame.image.load('cat0.png')

cat1Img = pygame.image.load('cat1.png')

#Game loop for quitting screen
running = True
while running:

    screen.fill((255, 255, 255))
    screen.blit(background, (0, 0))
    screen.blit(img, (490, 20))
    pygame.display.update()

    for event in pygame.event.get():
            if event.type == pygame.QUIT:
                running = False

