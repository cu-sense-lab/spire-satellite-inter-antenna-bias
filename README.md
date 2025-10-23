# spire-satellite-inter-antenna-bias
Inter-antenna (POD/RO) bias estimates for Spire LEMUR (currently 2023 only).

The file spire_ro_pod_bias_estimates_v0002.h5 contains the daily average biases and standard deviations (computed from raw arc-based bias estimates) in HDF5 format.
Estimates between each RO antenna and the POD antenna are provided.  The RO1/RO2 labels correspond to FRO/BRO or vice versa, as described in the paper.


Files inside `multipath-maps` contain the estimated multipath maps for P1/P2 observables for the POD and RO antennas.
The maps are binned according to the `bin_vertices`, which are cartesian coordinates on the unit sphere aligned to the satellite body frame.  They can be converted to az/el with:

az = arctan2(y, x)
el = arcsin(z)

