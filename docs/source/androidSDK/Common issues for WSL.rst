Common issues for WSL
==============.

1. CPU acceleration status: This user doesn't have permissions to use KVM (/dev/kvm)，ERROR: x86 emulation currently requires hardware acceleration!

        .. image:: ../../images/issues1.png
            :align: center

        |

        Follow the first solution in the `link <https://stackoverflow.com/questions/37300811/android-studio-dev-kvm-device-permission-denied>`_.
        Then, Just log in again.

        .. code-block:: bash

            sudo adduser $USER kvm
            sudo chown $USER -R /dev/kvm