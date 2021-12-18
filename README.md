# pim551
Pimoroni Pico RGB Keypad Base using CircuitPython on Raspberry Pi Pico

## Use GIT on CIRCUITPY
1. Clone this repository using `git clone git@github.com:bschapendonk/pim551.git --no-checkout <path-to-your-usual-place>` in your usual place (not on the CIRCUITPY device)
2. On your CIRCUITPY device create an `.git` file with the following content:
    ```
    gitdir: <path-to-your-usual-place>\.git
    ```
3. On your CIRCUITPY device run `git checkout main`

## Instal libraries using [CircUp](https://github.com/adafruit/circup)
1. Install CircUp
    * For Linux
        ```
        cd ~
        python -m venv .circuitpython
        source .circuitpython/bin/activate
        pip3 install circup
        ```
    * For Windows
        ```
        cd %USERPROFILE%
        python -m venv .circuitpython
        %USERPROFILE%\.circuitpython\Scripts\activate.bat
        pip3 install circup
        ```
2. Run `circup install -r requirements.txt` on your CIRCUITPY device 

## To erase CIRCUITPY
CircuitPython includes a built-in function to erase and reformat the filesystem.
1. Connect to the CircuitPython REPL using Mu or a terminal program.
2. Type the following into the REPL:

```python
import storage
storage.erase_filesystem()
```
