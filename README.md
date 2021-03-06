# Price-Check - A Hyperledger Fabric Application ![Hyperledger Fabric](https://img.shields.io/badge/Hyperledger%20Fabric-v1.4-E95248) ![Javascript](https://img.shields.io/badge/Javascript-JS-green)

Course Assignment for CS-2361: Blockchain and Cryptocurrencies 

Video demo of the application can be found here: https://youtu.be/8-eotu43IzY

## What is Hyperledger? 
Hyperledger is a permissioned blockchain network that can be locally bootstrapped. One can use the Hyperledger platform to create decentralized, permissioned applications. 

## What is PriceCheck? 
PriceCheck is an application that is based on the pre-existing "FabChat" application. A lot of the code has been derived from the FabChat chaincode. 

PriceCheck allows a user to list items for sale at a base price. Users can also propose an increase to the base price of an item which he must have listed earlier. But for the price-increase proposal to take effect, the following check must be passed: 50% of the total number of registered users must have already flagged (and hence, approved) the price increase. 

Once a price-increase proposal for an item receives sufficient approvals the base price of the said item is set to the increased amount. Lastly, every user should also be able to query the latest base price of any listed item.



[//]: # (SPDX-License-Identifier: CC-BY-4.0)

## Hyperledger Fabric Samples

Please visit the [installation instructions](http://hyperledger-fabric.readthedocs.io/en/latest/install.html)
to ensure you have the correct prerequisites installed. Please use the
version of the documentation that matches the version of the software you
intend to use to ensure alignment.

## Download Binaries and Docker Images

The installation instructions will utilize `scripts/bootstrap.sh` (available in the fabric repository)
script to download all of the requisite Hyperledger Fabric binaries and docker
images, and tag the images with the 'latest' tag. Optionally,
specify a version for fabric, fabric-ca and thirdparty images. If versions
are not passed, the latest available versions will be downloaded.

The script will also clone fabric-samples repository using the version tag that
is aligned with the Fabric version.

You can also download the script and execute locally:

```bash
# Fetch bootstrap.sh from fabric repository using
curl -sS https://raw.githubusercontent.com/hyperledger/fabric/master/scripts/bootstrap.sh -o ./scripts/bootstrap.sh
# Change file mode to executable
chmod +x ./scripts/bootstrap.sh
# Download binaries and docker images
./scripts/bootstrap.sh [version] [ca version] [thirdparty_version]
```

### Continuous Integration

Please have a look at [Continuous Integration Process](docs/fabric-samples-ci.md)

## License <a name="license"></a>

Hyperledger Project source code files are made available under the Apache
License, Version 2.0 (Apache-2.0), located in the [LICENSE](LICENSE) file.
Hyperledger Project documentation files are made available under the Creative
Commons Attribution 4.0 International License (CC-BY-4.0), available at http://creativecommons.org/licenses/by/4.0/.
