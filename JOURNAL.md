### 5/25: schematic p.1 (1.5hrs)
- i made an RP2040 board a while ago and it was super messy
- but now im a better PCB designer!
- lets try again
- going to follow https://pip-assets.raspberrypi.com/categories/814-rp2040/documents/RP-008279-DS-1-hardware-design-with-rp2040.pdf?disposition=inline
- ok features right now:
  - USB-C
  - neopixel (prob will not order cause expensive, so CANCEL THIS)
  - STEMMA-QT connector
  - panda shape
- lets get started w schematic

<img width="358" height="314" alt="image" src="https://github.com/user-attachments/assets/307f5b04-b273-4ae4-8bc4-ab35e196fc1f" />

- flash complete

<img width="393" height="229" alt="image" src="https://github.com/user-attachments/assets/76e8d348-fb9d-412f-a2b3-400514c87ef9" />

- voltage reg complete

<img width="407" height="239" alt="image" src="https://github.com/user-attachments/assets/bb34f9ca-3ade-4137-8ee8-62ef0b5c3f7a" />

- decaps done
- crystals + pins remaining

<img width="403" height="376" alt="image" src="https://github.com/user-attachments/assets/6e36fdd5-8756-480d-8899-ef846540267c" />

- added pins
- one thing that doesn't make sense to me is the fact that RP2040 has 30 GPIO yet Pico exposes only 26???? why?
- like i get its smaller but how much is 2 more GPIO on each side going to cost
- plus theres like 30 ground pins on 1 pico board... why?
- also if ur looking for small board you would get a Xiao, not a pico
- i genuniely do not understand why this is
- ok thats what im selling my board on

<img width="780" height="536" alt="image" src="https://github.com/user-attachments/assets/0555d043-1d37-4b19-b5f8-22f73c45d81c" />

- neatened up schematic!
- however, i cant seem to find the crystal footprint/symbol
- thats so weird
- ok will find out tmrw

### 5/26: schematic p.2 + PCB p.1 (1hr)
- going to add 2 STEMMA-QT connectors

<img width="591" height="377" alt="image" src="https://github.com/user-attachments/assets/e2d8dd63-1f47-4a33-8d93-791412196c8c" />

- added! there super easy to add

<img width="635" height="299" alt="image" src="https://github.com/user-attachments/assets/ecb0ae51-9baf-4c06-8a1e-66643527d1f6" />

- added crystal
- basically KiCAD updated the library in KiCAD 10 to merge pins 2 and 4 cause they both go to ground
- thats kind of confusing but ig it works
- asked in Slack for schematic review
- time for footprint assignments

<img width="728" height="562" alt="image" src="https://github.com/user-attachments/assets/b30483b7-5034-4878-bca4-8787b6761265" />

- done!
- time for PCB design

<img width="670" height="412" alt="image" src="https://github.com/user-attachments/assets/ba761c7e-f3f8-4240-97e3-92573d384003" />

- general placement

<img width="579" height="649" alt="image" src="https://github.com/user-attachments/assets/c6e86904-b2ee-4a67-96a1-85e256359983" />

- chat are we cooked
- ok im making the bottom and the top the same distance from one another such that RP2040 is perfectly in the middle
- nvm ill just make it wider

<img width="466" height="594" alt="image" src="https://github.com/user-attachments/assets/d938723d-1b12-4356-a696-1bb82efc832f" />

- uhhhhh it looks ugly
- not sure how to improve so ill start routing
