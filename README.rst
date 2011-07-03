========================================
Genetic Algorithms library for SC Server
========================================

(c) 2006 Dan Stowell


To install:
===========

Just drop this folder into your SuperCollider extensions 
directory (see the [Using-Extensions] helpfile for the 
location on your platform). 


To use:
=======

I'm afraid I haven't written any detailed instructions yet.
There is some information in comments stored in the top of
class files such as GAIsland, GAIndividual, GAGraphCreator2,
etc.

The "GA subclasses" folder contains example applications 
such as evolving to match a given envelope, evolving to 
match the pitch track of a given sound sample, etc.

Some of the "judge synths" make use of a UGen called 
"FFTDiffMags" which is available in my UGen pack.

See also my talk at the SC symposium 2006, available online
at http://www.mcld.co.uk/supercollider, which outlines some
background and examples.

To recap, here's a simple example of creative interactive
use of my GA library::

    s.boot;
    i = GAOwnDrone.new(server:s, numinds:24, channels:2).cullProportion_(0.2).makeGui;

 
Copyright:
==========

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation; either version 2
of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.


