# flo_chatRoom
Web Socket based chat room for FLO

There are 2 types of messages :
1. unicast - sends message only to a FLO_ID
2. broadcast - sends message to all in the chatroom


### To install :

    gcc chatRoomWSServer.c mongoose.c -o chatRoomWSServer
  
### To run the server :
 
    ./chatRoomWSServer
 
### Instructions :
 
1. Open `127.0.0.1:8000` in your web browser
2. To bind FLO_ID :
     `$self_FLO_ID`
3. To unicast message to a FLO_ID :
      `>receiverFLO_ID message`
4. To broadcast :
      `message`

 Note :
   You can receive unicast only if a FLO_ID is bound 