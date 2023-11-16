import os
import cfg
import sys
import pygame
import random
from modules import *


'''游戏初始化'''
def initGame():
    # 初始化pygame, 设置展示窗口
    pygame.init()
    screen = pygame.display.set_mode(cfg.SCREENSIZE)
    pygame.display.set_caption('catch coins —— 九歌')
    # 加载必要的游戏素材
    game_images = {}
    for key, value in cfg.IMAGE_PATHS.items():
        if isinstance(value, list):
            images = []
            for item in value: images.append(pygame.image.load(item))
            game_images[key] = images
        else:
            game_images[key] = pygame.image.load(value)
    game_sounds = {}
    for key, value in cfg.AUDIO_PATHS.items():
        if key == 'bgm': continue
        game_sounds[key] = pygame.mixer.Sound(value)
    # 返回初始化数据
    return screen, game_images, game_sounds


'''主函数'''
def main():
    # 初始化
    screen, game_images, game_sounds = initGame()
    # 播放背景音乐
    pygame.mixer.music.load(cfg.AUDIO_PATHS['bgm'])
    ...


'''run'''
if __name__ == '__main__':
    while main():
        pass
