
# APEX DMA
It's a DMA cheat framework for apex legends in VM.\
Based on Memprocfs, MicroVMI plugin( for leechcore ), and Memflow QEMU Connector.\
There's a simple example showing how to get key state and\
the health of LocalPlayer in this repo.

## Tested Features

- Keyboard (windows version > 22000) (Tested)
- CR3(DTB) Fix (Tested)
- Basic Memory Functions:
> - Scatter Read / Read (Tested)
> - Array Read (Tested)
> - Get Base Module Address / Size (Tested)
> - Scatter Write / Write (Not working)
> - Sig Scanning


## Use

```bash
  git clone https://github.com/atombottle/apex_dma.git
  sudo make
  cd build
  sudo ./apex_dma
```

Clean:
```bash
  sudo make clean
```

## TODO

- Fix Memory Write

- Test other features when I have time

- Windows with version <22000 will not be supported ( keyboard )\
  because the Registry is not working well\
  but modify winver in Memory/InputManager.cpp might work
  ( I don't have enough space for another VM so I can't test it)

## Credits

- DMA Library: https://github.com/Metick/DMALibrary
- LeechCore Plugin: https://github.com/ufrisk/LeechCore-plugins
- Memflow [Connector]: https://github.com/memflow/memflow-qemu 
- Memprocfs: https://github.com/ufrisk/MemProcFS


## Screenshot

![Screenshot](https://github.com/atombottle/apex_dma/blob/main/screenshots/pic.jpg)
