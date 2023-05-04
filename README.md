# Semana
Automation of space taking on Semana with github Actions schedule. All Monday at 00:30am, the script it's run to get your place on all days in 6 weeks.

## Installation

To get your information, open dev console and get the information in `POST` request to get your place.

- Fork this repo.
- Go to your `settings > Security > Secrets and variables > Actions` and add this :

  - `COLLABORATOR_ID` -> `your_collaborator_id`
  - `COOKIE` -> `your_cookie`
  - `DESK_ID` -> `your_desk_id`

Results :
![image](https://user-images.githubusercontent.com/13368283/225027727-ebe80f60-28d9-4c97-8a95-ecdaaca74884.png)

