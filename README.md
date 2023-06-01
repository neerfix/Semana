# Semana
Automation of space taking on Semana with github Actions schedule. All Monday at 00:30am, the script run to get your place on all days in 6 weeks.

## Installation

To get your information, open dev console and get the information in `POST` request to get your place.

- Fork this repo.
- Go to your `settings > Security > Secrets and variables > Actions` and add this :

  - `COLLABORATOR_ID` -> `your_collaborator_id`
  - `COOKIE` -> `your_cookie` (3 cookies is set by semana, take `sid` cookie value.
  - `DESK_ID` -> `your_desk_id`

### Get Informations

To get `collaborator_id`, `cookie` or `desk_id`. Open your navigator debugger (F12, or right clic, inspect element). 
Take your place one time and you can see in network tab, search `booking`. On tab `Payload`
![Sans titre](https://github.com/nick-notararigo/Semana/assets/13368283/858eb00b-7486-4e2c-801d-c9e172f8c330)

Results :
![image](https://user-images.githubusercontent.com/13368283/225027727-ebe80f60-28d9-4c97-8a95-ecdaaca74884.png)

