# OOAD-WEEK10
Sequence Diagram
##1.+<img src="http://www.plantuml.com/plantuml/img/ROx12e9048RlynH3zrx0GtGe8eg28ZhFkgCkwUwoErQ-VHeQALx_x-ERMKUX87LLGc4qO-QSAFS6CL8o7i-x_Gae5HVmTjrU47mhczHuieABEojFUQkvtDZ5Y1suKIxeqROX8KMH4U0RMwu6BJ7Mru8FRg1VEZZf9v6jHjr642QeiuVwd_RaOB86VdTdchqoq-jUJ6BXNbYHhJy0">
###@startuml
###hide footbox
###title LOGIN
###actor USER 
###participant "Webpage Login"
###participant Keybord
###participant Database 

###USER -> Keybord:input key
###Keybord -> "Webpage Login":send data 
###"Webpage Login" -> Database:send data verify
###Database -> "Webpage Login":verify
###"Webpage Login" -> USER:show manu

##2.<img src="http://www.plantuml.com/plantuml/img/LOjD3i8W48NtSugvW1TWOIInNMhYpm4eJYqfPGWCqUCNR3HnyPBtyxr35fEaB1uczo0ScMNWDuWJJtYE5B0t0OmLJdY_TXU4M7bdNJH1iDUdlpmK4Lu0FkHkttPb9x8pHb-U-EitJcNoP0L74wgom5P_ZqTzqr1Do-seNfncM040">
###@startuml
###hide footbox
###title Open Fan
###actor USER 
###participant FAN
###participant buttom

###USER -> FAN:check plug 
###USER -> buttom:select fan fast
###buttom -> FAN:DATA
###FAN -> USER:work

##3.<img src="http://www.plantuml.com/plantuml/img/ROvD2i8m48NtSugXUnTrcOK8ebj1smEawKX3fvEGJj7ZsmQq2jqzti_7Euvgaqu3G-TRmaS8seGNg5Scl4OIl5W1wpGahE_dM_cZzn3dhNS-Mb4iAcAANH128Ns6r1T_-JS6o23S7LRFd2mph8Gvs-2PaQH5cOQ64hfbiL5QjlcToOqiFrvfAiizm1i0">
###@startuml
###hide footbox
###title Open Fan
###actor USER1
###actor USER2
###participant "Telephone network"
###participant Telephone

###USER1 -> Telephone:Call
###Telephone -> "Telephone network":send number call
###"Telephone network" -> USER2:call
###USER2 -> USER1:Talk

##4.<img src="http://www.plantuml.com/plantuml/img/TOqn2uCm58JtzoiUxj8zGocbtLgGLfTkCRvYG4r8NehzzqsmA8AET_VTtScpT1pw3bhT4BwDuTgCm9exmjBOlB8W5Hk7rVFw01jXhRIL0sD97TdM3BHoCuwbOF5ineN8LiWGUYiRWBI8-V6lXO-qOlJaFbhH8RerEPZ2X6qlYuja2TjPQgKJKTnUM0J6UtI_y-_Eu0BkhyvAJ0W0_000">
###@startuml
###hide footbox
###title Top-Up
###actor USER
###participant Telephone
###participant "top-up Box Telephone"
###participant numpad

###USER -> numpad:select service/number
###numpad -> "top-up Box Telephone":Data
###"top-up Box Telephone" -> USER:PLZ Put Money
###USER -> "top-up Box Telephone":Put Money
###"top-up Box Telephone" -> Telephone:top-up

##5.<img src="http://www.plantuml.com/plantuml/img/ROrB3i8m34JtFeNLFMAV1K88Bi3d02OOrI8_DQvARqzI4A8LNixCUzvcfKvxxw2L6-CzHht69wYeOzmn1VHaMmaCP3LsU3aTZf0A8bOI1SNcTzGigYWEpnGUytmlEJaQ0QeCLvk5msHsRBLyvx1ElQAFWKUOZzxOrs_g63xYsbMr6KZq3pTr4pjHvLu0">
###@startuml
###hide footbox
###title Bean machine
###actor USER
###participant "Bean machine"
###participant "Boil Tank"
###participant Display

###USER -> "Bean machine":select Been/put money
###"Bean machine" -> "Boil Tank":Been
###Display -> USER:wait
###"Bean machine" -> USER:Boil Been

