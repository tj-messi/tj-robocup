# start

restart the linux environment for 24.04ubuntu lts

see the instruction in 

    https://docs.b-human.de/coderelease2024/getting-started/initial-setup/

## environment

    sudo apt upgrade

    sudo apt update

    sudo apt install ccache clang cmake exfatprogs git graphviz libasound2-dev libbox2d-dev libgl-dev libstdc++-12-dev llvm mold net-tools ninja-build pigz qt6-base-dev qt6-svg-dev rsync xxd

the limit of the decoding refer to csdn

    Make/Linux/generate

    Make/Linux/compile

## SimRobot

path

    /tj-robocup/tj-robocup/BHumanCodeRelease/Build/Linux/SimRobot/Develop

## gamecontroller3

download the release one

    https://github.com/RoboCup-SPL/GameController3/releases/tag/v3.0.0

get into the direct

    ./game controller

encounter the problem :

    /home/tj-messi/tj-robocup/tj-robocup/game_controller-3.0.0-x86_64-unknown-linux-gnu/target/release/game_controller_app: error while loading shared libraries: libwebkit2gtk-4.0.so.37: cannot open shared object file: No such file or directory

follow the csdn

## TeamCommunicationMonitor

    In addition, the GameController offers an interface for monitor applications (such as the TeamCommunicationMonitor or the EventRecorder):
    - It receives monitor requests (UDP unicast on port 3636, 4 bytes header magic `RGTr` + 1 byte version number `0`).
        It refuses to accept monitor requests from hosts that have previously sent status messages, as those are presumed to be robot players which should not get true data.
        Similarly, if a host that had previously sent a monitor request sends a status message, it will not receive monitor data anymore.
    - Each registered monitor host will get:
        - control messages with the true game state at a rate of 2 hertz (UDP unicast on port 3838, with the same format as regular control messages, but with the header magic `RGTD`).
        - forwarded status messages (UDP unicast on port 3940, prefixed by the IPv4 address of the original sender).
            The forwarded payload has not been validated.


first get the java environment

follow the csdn instruction