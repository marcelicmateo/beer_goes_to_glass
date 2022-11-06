# Custom made beer tower

## Opis proizvoda

In short: kada se toči pivo, postoje pokretni djelovi na točioniku koji se aktiviraju, krenu pokretati i ostaju aktivirani sve dok se pivo toči. Kada se pivo prestane točiti, aktivirani djelovi se gase, odnosno staju.

## Things to consider

From HW perspective:

- how to sense beer is being poored. (accelerometer seem as best idea, least intrusive, or water flow meter can be used, then pipes need to be retrofited with sensors)
- what motor to use, how strong, does it need speed or tork.
- LED?
- Digital sensors

From SW perspective

- Is SW modular, when designing, keep in mind parameters that change the behaviour of system
- User input, does it need to have any?
- Dashboard, do we need one?
- Remote contol of whole system, is it necessary?
- Does it need to be universal, or is it one time use?
- do we need server for remoe control?

## Quesion to designer

1. Imamo li pristup cijevima kojima teče piva? Ako da, možemo li onda njih koristiti za detekciju kada pivo teče ili ne?
2. Dali radimo svoju ručku točionika? Kako ukomponirati žice da ne smetaju bartener? Accelerometar za mjerenje kada se toči pivo. e.g. <https://www.hackster.io/26972/tap-tracker-smart-tap-handle-ae15ba>
3. Koliko velike su stvari koje se okreću, zubčanici? Pitanje je koliko jaki motor teba imati.
4. Koliko brzo se vrte stvari? high tork, low speed? Modularnost/podesivost?
5. Svejtla, dali postoje? Boja? Uzorak? Modularnost?

Na kraju krajeva, koliko cijeli sustav pokretanja djelova mora bit modularan? Dali je to sustav koji će se napraviti jednom i takav ostati zauvjek? Ili mora imati mogućnosti dodatne kontrole, mijenjanja nekakvih parametara (vrtnja, svjetla)?

## Selected tehnologies STUDY

- RPI 3 microcontroler all digital system
  Overkill if system is one time use and needs no modularity
  Has Linux, we can make everithing fully custumisible as we want.
  will need custom hats for controling HW
  can run Node red, development should be easier but maybe laggy
- accelerometer for detecting tap angle
- high tork motor
- LED strip?? needs defining

### BOM

| Item                                                                                                                                                                                                              | Price |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----- |
| [Accelerometre](https://www.chipoteka.hr/3-axis-digital-acceleration-sensor-module-mma8452-vma208-wpse208-9150036251) | 59,00kn |
| [Rpi3](https://www.chipoteka.hr/raspberry-pi-3-model-b-wifi-bluetooth-onboard-8208000130?search=raspberry%20pi&description=0) | 389,00kn  |
| servo| |
| LED| |