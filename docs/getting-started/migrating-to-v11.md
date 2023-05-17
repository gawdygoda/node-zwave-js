# Migrating to v11

I've put this off for a while now - we just got to a `.20` minor version for the first time.
But Z-Wave JS is on the road to certification, and some of those requirements are forcing my hand.

## Window Covering CC vs. Multilevel Switch CC

The `Window Covering CC` allows for more granular control of covers to the point of making `Multilevel Switch CC` redundant.
As a result, the Z-Wave specification forbids interacting with the `Multilevel Switch CC` on devices that support the `Window Covering CC`.

To avoid removing functionality for users, applications that plan on upgrading to `v11` must make sure to have support for the `Window Covering CC`.