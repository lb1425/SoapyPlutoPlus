# Soapy SDR module for Pluto+

## Installation instructions

```
sudo apt install libiio-dev
sudo apt install libad9361-dev
sudo apt install libusb-1.0-0-dev
sudo apt install libsoapysdr-dev
git clone  https://github.com/lb1425/SoapyPlutoPlus.git
cd SoapyPlutoPlus
mkdir build
cd build
cmake ..
make
sudo make install
```

## Dependencies

- [libiio](https://github.com/analogdevicesinc/libiio)
- [libad9361](https://github.com/analogdevicesinc/libad9361-iio)
- [SoapySDR](https://github.com/pothosware/SoapySDR)

## Documentation

* https://github.com/pothosware/SoapyPlutoSDR/wiki

Note that the Frequency Correction API is not implemented,
it's recommended that you adjust the `xo_correction` value with the observed PPM in the Pluto device `config.txt`.

## PothosSDR

Note that installation with PothosSDR is optional as "PlutoSDR SoapySDR binding (experimental)" and not selected by default.

This is due to possible problems with other libusb devices,
see [#24](https://github.com/pothosware/SoapyPlutoSDR/issues/24)
and [libiio#586](https://github.com/analogdevicesinc/libiio/issues/586)

## Licensing information

GNU LESSER GENERAL PUBLIC LICENSE Version 2.1, February 1999
