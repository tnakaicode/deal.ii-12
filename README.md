# Deal.ii Step-12

* DG method: Discontinuous Galerkin method
  * Discretization of the linear advection equation with the DG method.
    * $$\frac{\partial u}{\partial t} + c \frac{\partial u}{\partial x} = const$$
    * we have to distinguish the cases of boundary
      * regular interior faces
      * interior faces with hanging nodes
  * Assembling of the system matrix using the MeshWorker::loop().
    * <https://www.dealii.org/current/doxygen/deal.II/group__MeshWorker.html>
    * MeshWorker::loop() can distinguish between all the different faces.
