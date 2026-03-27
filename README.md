# ZMK Keyboard Config

## Configuration

Updates to keyboards are done within the `config` folder.
Select the {keyboard}.keymap to make changes to the given keyboard
Methods for configuring and references can be found [here](https://zmk.dev/docs/keymaps/list-of-keycodes)
Additionally, a good real example can be found [here](https://github.com/folke/zmk-config/blob/main/config/corne.keymap)

## Building Changes to the Keyboard

Once changes are completed you can push them to the Github which
is initialized with GH Actions that will build 2 artifacts that
represents the left and right side of the keyboard.
Once completed you can click on the job and download the artifact.

After extracting the artifact firmware from the download folder,
you're left with .uf2 files (one for each side of the keyboard).

Take your keyboard, find the small reset hole underneath the board
and click it once rapidly followed by an immediate long press (3s).
This should make the board discoverable by your file manager.
Upload the respective .uf2 file to the correct board (left/right).
Once the board disconnects automatically, the firmware is uploaded.
