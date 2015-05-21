Ref:lect is a Mir:ror user space driver. It publishes Mir:ror events on D-Bus.

# Design #

There are many solutions to continue to use the Mir:ror device. But, most of them run under Windows(TM).

First, Ref:lect runs on Linux.
Second, Ref:lect is designed around D-Bus system.
A single daemon communicates with the Mir:ror and published event on D-Bus service, allowing many different usages.

# Features #
Currently, the D-Bus service already offers enough operations to be quite usable.
Four signals allow to detect events such as: input or output of tag and flip up or down of the device.
Some operations allow to retrieve the list of currently landed tags.

An initial client, inspired by previous implementation called arewrim, runs as a daemon in the user's session. This daemon automatically calls some user's script based on event and tag.

As an example, it is possible to lock screen when a given tag is removed.

# Todo #
Many many ideas...

One of them is to login with just dropping a tag.