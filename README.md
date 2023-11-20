# scripts-localnetworkandexplorer
Magical scripts to start and stop Kurtosis and Docker when developping the explorer of beaconcha.in. They can fix some unexplained errors with Kurtosis and Docker, for example [this one](https://github.com/kurtosis-tech/kurtosis/issues/1769).

`./stop` will stop Kurtosis and Docker. The user can choose between 4 different strengths :
Level 1 is what the wiki says (_docker compose down && kurtosis engine stop_). The other levels force the removal of dockers, enclaves, services, caches... What is done depends on the strength level.
I do not recommend level 4, use it only if the other levels failed.
Level 5 has to be executed manually (not implemented): throw the computer into fire.

`./start` will start the local network and the explorer, following the instructions of the wiki. To do things properly, it calls first _stop_ (where the user needs a strength of 1 usually)

*Acknowledgements*

Thanks to [D13ce](https://github.com/D13ce) and [Rami](https://github.com/remoterami) and [gocoffeecup](https://github.com/gocoffeecup) for their help to exorcize my computer.

(test)

