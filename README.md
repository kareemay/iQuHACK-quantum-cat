# iQuHACK-quantum-cat
#iQuHACK quantum computing video game


import pygame

#initialize pygame
pygame.init()

#setting up screen dimensions
screen = pygame.display.set_mode((800,800))

#Title and Icon (work on later, have to download a pic first)
pygame.display.set_caption("Quantum Cat")
#icon = pygame.image.load('python')
#pygame.display.set_icon(icon)

#Cats
cat0Img = pygame.image.load('cat0.png')
cat0X = 100
cat0Y = 100

def cat0 ():
    screen.blit(cat0Img, (cat0X, cat0Y))

cat1Img = pygame.image.load('cat1.png')
cat1X = 85
cat1Y = 200

def cat1 ():
    screen.blit(cat1Img, (cat1X, cat1Y))

#Game loop for quitting screen
running = True
while running:

    screen.fill((255, 255, 255))

    cat0()
    pygame.display.update()

    cat1()
    pygame.display.update()

    for event in pygame.event.get():
            if event.type == pygame.QUIT:
                running = False
                
                
