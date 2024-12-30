# Expo Camera: Inconsistent onBarCodeScanned Callback

This repository demonstrates a bug in Expo's Camera API where the `onBarCodeScanned` callback is not always triggered reliably. The issue is particularly noticeable when scanning barcodes rapidly or using less common barcode formats.

## Bug Description

The `onBarCodeScanned` function within the Expo Camera component intermittently fails to fire. This inconsistency makes barcode scanning unreliable, and causes unexpected application behavior.

## Reproduction

1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Run the app using Expo Go.
4. Point the camera at a barcode and observe the inconsistent behavior of the `onBarCodeScanned` callback being triggered.

## Solution

The provided solution attempts to mitigate this issue by implementing more robust error handling and potentially adjusting the scanning interval or barcode types.