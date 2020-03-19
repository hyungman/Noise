# Noise

## Install VTK with following options turned on in cmake.

* Module_vtkFiltersParallelMPI
* Module_vtkRenderingParallel

## Building Noise
```
mkdir build
cd build
cmake -DVTK_DIR=/opt/vtk/lib/cmake/vtk-8.2 ..
```
## Running Noise

```
export LD_LIBRARY_PATH=/opt/vtk/lib
mpirun -n 4 apps/pvolume/pvnoise -r 128 128 128
```
