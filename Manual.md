  In vanilla file C:\Program Files\NVIDIA Corporation\NVIDIA GeForce Experience\www\app.js Add a new global variable (just below copyright notice)
	
 ```
 var ANONYMOUS_USER = {
   sessionToken: "dummySessionToken",
   userToken: "dummyUserToken",
   user: {
          userId: "",
          core: {
             birthdate: new Date(""),
             displayName: "",
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



