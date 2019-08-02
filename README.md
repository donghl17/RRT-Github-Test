# rrt_exploration_with_profiling_mapmerging_and_testing

this project is used by donghl17 during his summer_intern_2019 in nics_lab, tsinghua university

codes are changed and added based on the original version https://github.com/hasauino/rrt_exploration
and codes are kept updating


some changes we make:
1.add a new case of two_robot in the scenario of house
2.add some codes used for profiling but now they are all noted
3.add a package named "testrrt",written in c++, whose function is to load a .bag file and publish them on the topic.you can use it while you are debugging
4.rewrite the "mapmerge" package based on http://wiki.ros.org/multirobot_map_merge. the package is not finished yet and if you want to use it, please use the command “rosrun mapmerge_test mapmerge_test_dhl”.this node should be run when you roslaunch the "two_simulated_house.launch" or "mutliple_simulated_largeMap.launch" and some parameters need to be changed.


what we will do in the future:
1.add a .launch file for the mapmerge package(seeting some parameters for a better API)
2.make the codes more user-friendly~
3.although slam can be down in the lastest version, donghl are still confused about some phenomenon
4.add some new function in the mapmerge package.(for example：rotating)
