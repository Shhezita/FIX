  In vanilla file C:\Program Files\NVIDIA Corporation\NVIDIA GeForce Experience\www\app.js Add a new global variable (just below copyright notice)
	
 ```
 var ANONYMOUS_USER = {
   sessionToken: "dummySessionToken",
   userToken: "dummyUserToken",
   user: {
          userId: "XXXXXXXX",
          core: {
             birthdate: new Date("1900-01-01"),
             displayName: "XXXXXXXX",
             primaryEmailVerified: true
          }
      }
 };
 ```
Then find
    
    return u.info("main.auth resolved called"),
	
 and replace by
 
    return u.info("main.auth resolved called"), n.hasSession = function(){return !0;}, n.getLoggedInUser = function(){return ANONYMOUS_USER.user;}, n.getSession = function(){return ANONYMOUS_USER;},

Find (x4):

    .isShareSupported=

Replace (x4):

    .isShareSupported=!0,

<p align="center">
  <img src="https://github.com/Shheza/Fixy/assets/32721494/f2e2674a-3250-402f-ba5a-e695b07cdd75" />
</p>

