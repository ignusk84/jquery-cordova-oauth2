This project is completely based on https://github.com/krisrak/jquery-cordova-oauth2.

It basically allows easier integration with JSPM and Typescript by wrapping the code in a module.

You can install it by running the following:

jspm install $oauth2=github:ignusk84/jquery-cordova-oauth2

to use the module, refer to the origninal plugin for documentation, but

$.oauth2() has been replaced by  $oauth2.request()

In typescript, you can include include using:

import * as $oauth2 from "$oauth2";

with the following typing:

declare var $oauth2: any;
declare module "$oauth2" {
    export = $oauth2;
}
