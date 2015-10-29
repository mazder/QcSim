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
* Usage: At least two argumets must be provided to run targetGen
* The name of trace file to be generated ( such as traceFile.trace)
* The name of class list file to be generated (such traceFile.cls)

# # Example: $./targetGen traceFile.trace traceFile.cls

