-- Stackedit xpecto Readme --

depencies:
    - nodejs (>= v0.10.33) http://nodejs.org/
    - npm (>= 1.4.28, https://www.npmjs.com/package/npm)
    - bower (npm install --global bower) >= 1.3.12
    - gulp  (npm install --global gulp)  >= 3.8.10

    stackedit and gatekeeper are also needed:
       git clone https://github.com/xpecto/stackedit
       git clone https://github.com/prose/gatekeeper


install:
    stackedit:
        cd stackedit && npm install && bower install
            (possible that the RobinThift commit is still gone and npm
             fails, if so remove the hash from package.json file)
    gatekeeper:
        cd gatekeeper && npm install


run:
    stackedit:
        gulp && node server.js
    gatekeeper:
        adjust config.json (oauth client Id and secret are needed)
        node server.js


infos:
    info about stackedit:
        https://github.com/benweet/stackedit/blob/master/doc/developer-guide.md#developer-guide
        https://github.com/benweet/stackedit
    info about gatekeeper:
        https://github.com/prose/gatekeeper
