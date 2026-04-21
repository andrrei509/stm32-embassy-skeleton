# STM32U545RE Embassy Skeleton

This is a staple/skeleton project for embedded Rust development on the **STM32 Nucleo-U545RE-Q** development board. It is pre-configured to use the asynchronous **Embassy** framework and **defmt** for logging.

## Prerequisites

Before using this project, ensure your computer has the necessary tools installed:

1. **Rust Toolchain:** Install Rust via [rustup](https://rustup.rs/).
2. **Architecture Target:** The STM32U545 requires the ARMv8-M target. Install it by running:
   `rustup target add thumbv8m.main-none-eabihf`
3. **Flashing Tool:** Install `probe-rs` to flash and debug the firmware:
   `cargo install probe-rs-tools`

## How to Start a New Lab

To use this skeleton for a new lab or project, follow these steps:

1. **Duplicate** this folder and rename it to your new project's name (e.g., `lab05`).
2. Open `Cargo.toml` in the new folder and change the `name` field to match your project name.
3. Open `src/main.rs` and start writing your code!

## Running the Code

1. Connect the STM32 Nucleo-U545RE-Q board to your computer. **Important:** Make sure you use the **USB-C STLK port** on the board, not the USB USER port.
2. Run the following command to compile the code, flash it to the board, and open the log console:
   ```bash
   cargo run
