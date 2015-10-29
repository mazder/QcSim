# TraceFileGen

# Obtaining TraceFileGen
TraceFileGen can be downloaded from https://github.com/GarCoSim/TraceFileGen

# Required Dependencies
  TraceFileGen has the following requirements
  * CMake is required to compile the sources. CMake can be obtained from https://cmake.org/
  * g++ (GCC) 4.4.7 or newer is required to compile the sources, visit https://gcc.gnu.org/

# Overview of the Directories Structure
  The following table lists the names of all directories and a short description.
  <table>
  <tbody>
    <tr>
      <td>
      <div>Name</div>
      </td>
      <td>
      Description.
      </td>
      </tr>
    <tr>
      <td>
      <div>build</div>
      </td>
      <td>
      build folder which is created by the ./build.sh script 
      </td>
      </tr>
    <tr>
      <td>
      <div>ObjectClasses</div>
      </td>
      <td>
      C++ sources
      </td>
      </tr>
    <tr>
      <td>
      <div>Utils</div>
      </td>
      <td>
       C++ sources 
      </td>
      </tr>
  </tbody>
  </table>
  
# Installation (Initial Builing)
  After downloading followed by extracting or cloning, do the followings
  * $ cd TraceFileGen
  * $ ./build.sh

# Compiling (After Initial Build)
  After intial building, do the followings
  * $ cmake ..
  * $ make
  
# Running (targetGen - the executatble in the build folder)
Usage: At least two argumets must be provided to run targetGen
* The name of trace file to be generated ( such as traceFile.trace)
* The name of class list file to be generated (such traceFile.cls)
Example: $./targetGen traceFile.trace traceFile.cls
Options:

Arguments		Short	Description

  ----------------------------------------
  
  --iteration x	  	-i x	x number as the number of iterations (default: 100)
  
  --thread x		-t x	x number as the number of threads (default: 10)
  
  --class x			-c x	x number as the number of classes (default: 300)
  
  --pointers x		-p x	x number as the maximum number of pointer fields in objects/static pointer fields in classes (default: 10)
  
  --primitives x	-pm x	x number as the maximum number of primitive fields in objects/static primitive fields in classes (default: 6)
  
  --allocation x	-a x	x percent as the allocation (default: 2)
  
  --storeaccess x	-s x	x percent as the store (default: 10)
  
  --readaccess x	-r x	x percent as the read (default: 88)
  
  --deleteroot x	-d x	x percent as the rootdelete (default: 10)
  
  --static x		-sf x	x percent as the static field access (default: 30)
  
  --prifaccess x	-pfa x	x percent as the primitive field access (default: 70)
  
  --classaccess x	-ca x	x number as the maximum used a class to create objects (default: 300)
  
  --escape x		-e x	x probability as the an object to be escaped (default: 20)
  
  --esctopartner x	-etp x	x probability as an object to be escaped to partner thread (default: 90)
  
