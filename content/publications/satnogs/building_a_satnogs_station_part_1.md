+++
date = '2025-08-30T21:13:46+03:00'
draft = false
title = 'Building a SatNOGS station: hardware setup'
tags = ["satnogs", "ground station"]
topics = ["SatNOGS"]
[rtwt]
 sidePane = true
 sidePaneSticky = true
+++

# Building a SatNOGS station

This article is the first part of the series about building a SatNOGS groundstation.
It will address hardware considerations, setup and testing. The second article will focus more onto the software, how to setup a SatNOGS client.
The third and last article will illustrate more advanced usages.

## Antenna setup

This station will use both VHF and UHF V-dipole antennas.

![V-dipole antenna](https://s1.qwant.com/thumbr/474x355/1/d/9197639e3a09f197e8b4c941790029d3c4c008e892a81bdc5ee056247da596/OIP.DBrwqEsLMi3ZJtcjIW73PwAAAA.jpg?u=https%3A%2F%2Ftse.mm.bing.net%2Fth%2Fid%2FOIP.DBrwqEsLMi3ZJtcjIW73PwAAAA%3Fpid%3DApi&q=0&b=1&p=0&a=0)

The UHF antenna will have a ground plane added to improve directivity, improving gain and decreasing interferences from the ground. The VHF antenna will not because of volume constraints.

## LNA and VHF-UHF diplexer

LNAs are used for both bands to improve the reception SNR. The UHF antenna directivity was improved so it will hopefully not cause the SDR device to saturate.

The diplexer S-parameters were verified and offer good performance.

## Airspy R2

The SDR device will be an Airspy R2 connected to a Beelink S13. The Airspy R2 has a fixed sample rate of 10 Msps, although there is an option to run it at 2.5 Msps.

![Airspy R2](https://s2.qwant.com/thumbr/474x474/6/d/0a98419d2cd9ad2057004404f0885935ed4247ef145404a880aedea0f1f04c/OIP.q9O93wET0VXzrDVKWZNRfgHaHa.jpg?u=https%3A%2F%2Ftse.mm.bing.net%2Fth%2Fid%2FOIP.q9O93wET0VXzrDVKWZNRfgHaHa%3Fr%3D0%26pid%3DApi&q=0&b=1&p=0&a=0)
