# U.S. Prosecutor Database
## DATA
> Last Updated: November 2nd 2019

This is the `csv-json-data` branch for manually collecting data.

### Installation

1. `git clone git@github.com:billimarie/prosecutor-database.git`
2. `cd [repo]/csv-json-data`
3. `git checkout -b [state]-[role]`
4. first time only: `npm install`
5. first time only: `npm install -g csvtojson`

### Instructions

1. Create a new .csv file as `[state]-[role].csv`. Add the **Basic Prosecutor Profile** columns:

* Name
* Location (State, County)
* Role
* Website
* Office Info (Address)
* Contact Info (Phone, Fax, Email)
* Optional: headshot / profile image (url)

*Note: You can always add additional columns, as long as it conforms to the Full Prosecutor Profile (Demographics: Age, Race, Gender, Party).*

2. Google your chosen state's prosecutor association.

3. Collect the data in your .csv file. **Remember: One State, One Role, One Branch.**

4. Run the `csvtojson` Node module (ex: `ny-da.csv > ny-da.json`): `csvtojson [state-role].csv > [state-role].json`

5. Be mindful of isolating your work. **As always: One State, One Role, One Branch.**

6. Add, Commit, and Submit a Pull Request:

```
git add .
git commit -m "Added [state] [role] as .csv and .json"
git push origin [branch]
```
