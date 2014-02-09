readsmscalls
============

Read SMS and Calls with Phonegap 2.3

Forked From:
https://github.com/dimitrismistriotis/ReadSmsCordovaPlugin

TODO: Proper fork and documentation

Code Sample
==========
    /* 
      @param callback - will be called after a successfull request
      @param number - Phonenumber to search for
      @type - "GetTexts", "GetCallLog", "GetSentTexts", etc.
      @Description - See Java file for detailed list of methods.
    */
    var readDeviceLog = function (callback, number, type) {
            cordova.exec(function (winParam) {
                callback(winParam, false);
            }, function (error) {
                console.log("CallLog Read Error");
            }, "ReadSms", type, [number]);
        }
