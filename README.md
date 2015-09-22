# JSON example assignment

The backend server has 2 endpoints that you need to interface with. Details are below.

### GET /get-problem/<netid>

Get a new problem to solve. You must put your netid where <netid> is in the URL.

Response from the server will be JSON-encoded with a message and a list of numbers. These numbers are unique per person and randomly generated each time this is called.

### POST /submit-answer

Submit your answer to the problem retrieved. This endpoint must be called within 3 seconds with the correct answer or you will need to restart.

Your answer must be JSON-encoded with the following parameters:

|Parameter|Type|Explanation|
|---------|----|-----------|
|netid|str|Your netid|
|answer|int|Your answer to the problem from `/get-problem`|

## Suggestions

Read up on using the [Requests library](http://www.python-requests.org/en/latest/) and the [JSON library](https://docs.python.org/2/library/json.html). 

Your program should be written in Python 2. For the differences between Python 2 and 3, read up on it [here](https://wiki.python.org/moin/Python2orPython3).

If anything is unclear, feel free to ask questions on Slack.
