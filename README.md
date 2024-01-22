![GitHub forks](https://img.shields.io/github/forks/nick-notararigo/semana)
[![Get my place on Semana](https://github.com/nick-notararigo/Semana/actions/workflows/schedule.yml/badge.svg)](https://github.com/nick-notararigo/Semana/actions/workflows/schedule.yml)
# Semana
Automation of space taking on Semana with github Actions schedule. All Monday at 00:30am, the script run to get your place on all days in 6 weeks.

## Installation

To get your information, open dev console and get the information in `POST` request to get your place.

- Fork this repo.
- Go to your `settings > Security > Secrets and variables > Actions` and add this :

  - `COMPANY` -> if you want set your place for 'cospirit' company, set value at `cospirit`. (You can find it in Url of your semana's company)
  - `COLLABORATOR_ID` -> `your_collaborator_id`
  - `COOKIE` -> `your_cookie` (3 cookies is set by semana, take `sid` cookie value.
  - `DESK_ID` -> `your_desk_id`
  - `DESK_ID_[0-4]` -> Change your desk on specific days of weeks (0 = monday; ... ; 4 = friday). If `DESK_ID_[0-4]` exist, is use in script, else use default `DESK_ID`
  - `STATUS` -> Set by default `6a0dffcb-5ab3-4108-9fde-4a834eeb8d9e` (On local company)
  - `STATUS_[0-4]` -> Same as `DESK_ID_[0-4]`, you can specify a day to remote with this value : `28b83f47-0221-4dac-b3c0-f6a8690e64b3`

### Get Informations

To get `collaborator_id`, `desk_id`. Open your navigator debugger (F12, or right clic, inspect element). 
Take your place one time and you can see in network tab, search `booking`. On tab `Payload`
![Sans titre](https://github.com/nick-notararigo/Semana/assets/13368283/858eb00b-7486-4e2c-801d-c9e172f8c330)

To get your cookie, follow this screen and copy the red rectangle
![Sans titre (2)](https://github.com/nick-notararigo/Semana/assets/13368283/5b880c94-5b89-406f-a224-6f643d9d73d9)

Results :
![image](https://user-images.githubusercontent.com/13368283/225027727-ebe80f60-28d9-4c97-8a95-ecdaaca74884.png)

