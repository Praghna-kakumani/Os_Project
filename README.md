# Os_Project

IndianRail has decided to improve its efficiency by automating not just its trains but also its passengers. Eachpassenger and each train is controlled by a thread. You have been hired to write synchronization functions that will guarantee orderly loading of trains. I have  defined a structure struct station, plus several functions described below.When a train arrives in the station and has opened its doors, it invokes the function station_load_train(struct station *station, int count)
where count indicates how many seats are available on the train. The function must not return until the train issatisfactorily loaded (all passengers are in their seats, and either the train is full or all waiting passengers have boarded).When a passenger arrives in a station, it first invokes thefunction station_wait_for_train(struct station *station)This function must not return until a train is in the station (i.e., a call to station_load_train is in progress) and there are enough free seats on the train for this passenger to sit down and I have used this for that train on the board tells us more information(station_on_board(struct station *station)) I have created a file of Create a file IndianRail.c the above three functions contains the declarations of the structure i used function station_init, which will be invoked to initialize the station object when IndianRail boots. by using this locks

● lock_init (struct lock *lock)
● lock_acquire(struct lock *lock)
● lock_release(struct lock *lock)
● cond_init(struct condition *cond)
● cond_wait(struct condition *cond, struct lock *lock)
● cond_signal(struct condition *cond, struct lock *lock)
● cond_broadcast(struct condition *cond, struct lock *lock)
