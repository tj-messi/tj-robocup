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