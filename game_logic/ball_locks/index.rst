Ball Locks
==========

+------------------------------------------------------------------------------+
| Related Config File Sections                                                 |
+==============================================================================+
| :doc:`/config/ball_locks`                                                    |
+------------------------------------------------------------------------------+

MPF's *ball locks* are used to hold a ball that has entered a
:doc:`/mechs/ball_devices/index` towards multiball.

.. note::

   If you just want to temporarily hold a ball while something else is happening
   (like during a video mode or while some award show is playing), use MPF's
   ``ball_holds:`` section, not a ball lock.

Ball locks are "logical" (not physical), so different ball locks can exist in
different modes that hold balls in the same device (depending on what mode is
running).

Ball lock devices track the number of balls "locked" on a per-player basis, so
even if one player empties out a physical ball device, the ball lock for another
player will know how many balls that player had locked, even if the number of
balls in a contained physical ball device doesn't match.

You can have lots of different ball locks in your game, typically configured
per mode.

+------------------------------------------------------------------------------+
| Related How To Guides                                                        |
+==============================================================================+
| TODO                                                                         |
+------------------------------------------------------------------------------+

+------------------------------------------------------------------------------+
| Related Events                                                               |
+==============================================================================+
| :doc:`/events/ball_lock_name_balls_released`                                 |
+------------------------------------------------------------------------------+
| :doc:`/events/ball_lock_name_full`                                           |
+------------------------------------------------------------------------------+
| :doc:`/events/ball_lock_name_locked_ball`                                    |
+------------------------------------------------------------------------------+
