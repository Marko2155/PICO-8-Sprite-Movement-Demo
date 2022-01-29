# PICO-8-Sprite-Movement-Demo
Just a demo for sprite movement in PICO-8.
Code:
function _init()
player_sprite=1
player_x=64
player_y=100

gravity=1
end

function _update()
if btn(0) then
 player_x-=2 end

if btn(1) then
 player_x+=2 end
 
if btn(2) then
 player_y-=2 end

if btn(3) then
 player_y+=2 end
end

function _draw()
  cls()
  map(0,0,0,0)
  spr(player_sprite,player_x, player_y)
  print("                ")
  print("                ")
  print("       arrow keys to move        ")
  print("          esc to close           ")
end
PICO-8: https://getintopc.com/softwares/game-maker/pico-8-free-download/
You can trust the link and website even if it looks fishy.
