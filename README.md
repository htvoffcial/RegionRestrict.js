# RegionRestrict.js
For developing Access Region Restrict.Static Client JavaScript.

## How to USE.
### request method
```
REGIONRESTRICT("type",["countryCode(2)"],callbackaction);
```
### reference
| key | value | require |
| --- | --- | --- |
| type | text(String) | yes |
| countryCode(2) | text(Array) | yes |
| callbackaction | function | no |
### keys

#### type
This key is adopt access accept type.

(Examples)

allow:this access accept type is whitelist verdict.

deny:this access accept type is blacklist verdict.

#### countryCode(2)
This key is setting country with ISO 3166-1 applicable to type.

(Examples)

JP:Japan

US:UnitedStates

RU:Russia Federation

#### callbackaction
This key is callback function that when as stated above conditions.

### demo&example code
#### example code
This code is examples for accessible only "Japan","United States","Russia Federation".
```
var region_restrict_allow_list = ["JP","US","RU"];
REGIONRESTRICT(“allow”,region_restrict_allow_list);
```
#### results
