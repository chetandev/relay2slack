systemd
=======

To run relay2slack in systemd, perform the following steps:

Use the provided unit files. For most systems, the main unit file is placed at `/etc/systemd/system/relay2slack.service` (your mileage may vary).

Next, create the directory `/etc/systemd/system/relay2slack.service.d` and place `proxy.conf` inside.

Once the unit files are in place, reload systemd configuration with `systemctl daemon-reload`.

To run the server, use `systemctl start relay2slack`.

If you would like relay2slack to start on system boot, run `systemctl enable relay2slack`.
