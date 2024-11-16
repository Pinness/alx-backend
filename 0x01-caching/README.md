# FIFO Caching System

This project implements a FIFO (First-In-First-Out) caching system using Python. The `FIFOCache` class inherits from `BaseCaching` and follows the FIFO algorithm to manage a fixed-size cache.

## Features

- Adds and retrieves items in a cache using FIFO rules.
- Automatically discards the oldest item when the cache exceeds its size limit (`BaseCaching.MAX_ITEMS`).
- Outputs the discarded key when an item is removed.

## Class: FIFOCache

### Methods

1. **`put(self, key, item)`**
   - Adds an item to the cache.
   - Discards the oldest item if the cache size exceeds `MAX_ITEMS`.
   - Prints `DISCARD: <key>` for the discarded key.

2. **`get(self, key)`**
   - Retrieves the value associated with a key.
   - Returns `None` if the key is not in the cache or if the key is `None
