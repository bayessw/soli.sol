// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract Counter {
    int public count;

    // Sayacı 1 artır
    function increment() public {
        count += 1;
    }

    // Sayacı 1 azalt
    function decrement() public {
        count -= 1;
    }

    // İstediğin kadar artır
    function add(int x) public {
        count += x;
    }

    // İstediğin kadar azalt
    function subtract(int x) public {
        count -= x;
    }

    // Reset
    function reset() public {
        count = 0;
    }

    // Current value
    function getCount() public view returns (int) {
        return count;
    }
}
