# CHIP-0007 JSON FORMAT GENERATOR

This project converts each row in a CSV into it's CHIP-0007 JSON format equivalent. for each row, a JSON file is created, and saved in your directory. Furthermore, the hash of the json file from each row of the csv is calculated and appended as a new column to an output csv.
NOTE: JSON files are generated for each row.
a csv file is also generated with name filename.output.csv, where filename represents the name of your initial csv

## Acknowledgements

- [HNGi9](https://internship.zuri.team/hngi9)

## Run Locally

Clone the project

```bash
  git clone https://github.com/olanipekun01/nft_task_eyitayo.git
```

Go to the project directory

```bash
  cd nft_task_eyitayo
```

create and activate your virtual environment. for windows use the command below. for other users, please check how to activate a virtual environment on your OS.

```bash
virtualenv environment_name
environment_name/Scripts/activate
```

Install the required package

```bash
pip install -r requirements.txt
```

run the code

```bash
python main.py
```

## Running Tests

To run tests, run the following command

```bash
  python main.py
```

## Example output

```bash
{
    {
    "format": "CHIP-0007",
    "name": "alli-the-queeny",
    "description": "Alli is an LGBT Stan.",
    "minting_tool": "TEAM BEVEL",
    "sensitive_content": false,
    "series_number": 2,
    "series_total": 420,
    "attributes": [
        {
            "trait_type": "hair",
            "value": "bald"
        },
        {
            "trait_type": "eyes",
            "value": "white"
        },
        {
            "trait_type": "teeth",
            "value": "none"
        },
        {
            "trait_type": "clothing",
            "value": "yellow"
        },
        {
            "trait_type": "accessories",
            "value": "mask"
        },
        {
            "trait_type": "expression",
            "value": "none"
        },
        {
            "trait_type": "weakness",
            "value": "none"
        }
    ],
    "collection": {
        "name": "Zuri NFT Tickets for Free Lunch",
        "id": "b774f676-c1d5-422e-beed-00ef5510c64d",
        "attributes": [
            {
                "type": "description",
                "value": "Rewards for accomplishments during HNGi9."
            }
        ]
    }
}
```

## Tech Stack

**Server:** Python (Version 3.10.4)