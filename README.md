# wg-peer

An absolutely bare-bones WireGuard peer container meant to be deployed however you wish.

## Usage

Build image:

    $ docker build wg-peer:latest .

Run container:

    $ docker run --cap-add net_admin -v wg0.conf:/etc/wireguard/wg0.conf wg-peer:latest