# libRSF - A Robust Sensor Fusion Library
#
# Copyright (C) 2018 Chair of Automation Technology / TU Chemnitz
# For more information see https://www.tu-chemnitz.de/etit/proaut/self-tuning
#
# libRSF is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#
# libRSF is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with libRSF.  If not, see <http://www.gnu.org/licenses/>.
#
# Author: Tim Pfeifer (tim.pfeifer@etit.tu-chemnitz.de)

add_executable(ICRA19_Ranging ICRA19_Ranging.cpp)
target_link_libraries(ICRA19_Ranging ${CERES_LIBRARIES} libRSF)

add_executable(ICRA19_GNSS ICRA19_GNSS.cpp)
target_link_libraries(ICRA19_GNSS ${CERES_LIBRARIES} libRSF)

add_executable(IV19_GNSS IV19_GNSS.cpp)
target_link_libraries(IV19_GNSS ${CERES_LIBRARIES} libRSF)
