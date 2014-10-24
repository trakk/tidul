# TiDuL #

Time and Duration Programming Language, used in other trakk projects

## Purpose ##

The purpose of TiDuL is to provide a simple and idiomatic way of representing 
complex time calculations. While mechanical time is counted steadily off in 
seconds since an epoch, many real-world scheduling tasks for human or business 
purposes are better expressed in a variety of cycles and markers. Further, the 
details of calculating lunar cycles, religious holidays, civil holidays, and 
other dervied events are seldom germane to the application code that relies on
the results. 

## Specifying Date(time)s ##

All time calculations in a TiDuL program are relative to the program's defined 
Base Time. By default the Base Time is equal to Now when evaluation of the 
expression begins. If the base time is redefined all subsequent calculations 
will occur as if the program were run at that time instead.

## Specifying Periodicity ##

Another key problem solved with TiDuL is finding out a series of times based on
some recurring pattern.

* ODD/EVEN P: alternating P, starting with the 1st (ODD), or 2nd (EVEN) 
* N(th|nd|st) P: 
* DAY OF WEEK: SUNDAY,MONDAY,TUESDAY,WEDNESDAY,THURSDAY,FRIDAY,SATURDAY
<br>**NOTE**: starting day of the week, and numeric value of each day of the 
week are configurable (see configuring TiDuL)

## Claiming Results ##

For periodic dates, multiple or infinite results can be found, depending on 
whether there is an end time specified in the calculation.

* Single Time: Formating?
* Array of Times
* Count of matching times: 
* Warnings and Errors: Undefined future times, Overflows


# Copying #

Copyright (C) 2014  David Ulrich

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published
by the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
