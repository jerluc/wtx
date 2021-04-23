# Introduction

HTTP is the _hypertext transfer protocol_, which describes a simple, text-based \(vs. binary\) protocol for sending data over the web. Using this protocol, most web interactions are modeled as a cycle of _requests_ from _clients_ to _servers_ which reply with _responses_.

For example, when you go to a web page, e.g. [jerluc.com](https://jerluc.com), there are several resources in addition to the page text that need to be downloaded in order to render the page to your computer screen, e.g. images, icons, fonts, etc. Your web browser \(the _client_\) requests each of these resources individually from jerluc.com \(the _server_\), which then replies with the data. Once the response has been downloaded, your browser then compiles the information together into a displayable view which is what we see on our screens. Lastly, when you click on a web link on the web page, the cycle starts all over again.

This simple interaction is only the beginning of the many ways in which HTTP is used in modern software.

