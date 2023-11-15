# scripts-localnetworkandexplorer
Magical scripts to start and stop Kurtosis and Docker at Bitfly for the explorer. They can fix some weird errors, for example [this one](https://github.com/kurtosis-tech/kurtosis/issues/1769).

`./stop` will stop Kurtosis and Docker. The user can choose between 4 different strengths :
Level 1 is what the wiki says (_docker compose down && kurtosis engine stop_). The other levels force the removal of dockers, enclaves, services, caches... What is done depends on the strength level.
I do not recommend level 4 unless you are desperate as I have been because the other levels failed.

`./start` will start the local network and the explorer, following the instructions of the wiki. To do things properly, it calls first _stop_ (where the user needs a strength of 1 usually)
