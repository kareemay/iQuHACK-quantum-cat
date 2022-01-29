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


#Game loop for quitting screen
running = True
while running:
    for event in pygame.event.get():
            if event.type == pygame.QUIT:
                running = False

