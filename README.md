## Commands and outputs

## docker-compose up
detector_1   | streaming.transactions.legit {'source': 'nQanpKaMgBdg', 'target': '38GBylr8zGe2', 'amount': 53.69, 'currency': 'USD'}
detector_1   | streaming.transactions.legit {'source': 'LkoP3YLIsyeB', 'target': '5aMxMtynCiWt', 'amount': 247.09, 'currency': 'USD'}
detector_1   | streaming.transactions.legit {'source': 'u0BNW7NxeByc', 'target': '0UIhUJrpJoSG', 'amount': 808.46, 'currency': 'USD'}
detector_1   | streaming.transactions.fraud {'source': 'rd13lqteC9tG', 'target': 'E5Nv4704OZYI', 'amount': 916.76, 'currency': 'USD'}
generator_1  | {'source': 'jb2Mb2HJs0ci', 'target': 'xuO6fREnkCvQ', 'amount': 210.01, 'currency': 'USD'}
generator_1  | {'source': '4b8OScJ4yFk0', 'target': '6HN9pGnva4AM', 'amount': 202.09, 'currency': 'USD'}
generator_1  | {'source': '1TMPOwVgHpvO', 'target': 'egTsoShs33Wo', 'amount': 876.79, 'currency': 'USD'}

## docker-compose -f docker-compose.kafka.yml exec broker kafka-console-consumer --bootstrap-server localhost:9092 --topic streaming.transactions.legit --from-beginning
{"source": "KuNHpTZd49A9", "target": "Pj4OntV7Uwc2", "amount": 246.32, "currency": "USD"}
{"source": "hV0mYRb7NeW7", "target": "9WZyA4xERW1e", "amount": 524.93, "currency": "USD"}
{"source": "KIHbfa7JSNss", "target": "esLCLjtkSG14", "amount": 678.1, "currency": "USD"}
{"source": "GwIZf2OViWV1", "target": "5iuEXlTXMqtd", "amount": 122.13, "currency": "USD"}
{"source": "ObfqgUXVEua6", "target": "3e69LHDsNDio", "amount": 684.83, "currency": "USD"}
{"source": "CCYhyQBdr6cu", "target": "uVn1OAVshL2o", "amount": 602.66, "currency": "USD"}
{"source": "NzaB2eVEV1WA", "target": "jcctqeosvUfK", "amount": 621.95, "currency": "USD"}

## docker-compose -f docker-compose.kafka.yml exec broker kafka-console-consumer --bootstrap-server localhost:9092 --topic streaming.transactions.fraud --from-beginning

{"source": "YJRqVYtNYTvI", "target": "aUqi4D0ND5jA", "amount": 939.3, "currency": "USD"}
{"source": "CokX4IgchzaM", "target": "InxYVXXawYE3", "amount": 972.79, "currency": "USD"}
{"source": "4GJOtZBjJ1Bi", "target": "633Dz5cJQWOI", "amount": 961.04, "currency": "USD"}
{"source": "EnU2tuut7fSx", "target": "NsEV8qg4NYnu", "amount": 920.05, "currency": "USD"}
{"source": "4dvxi7jyp6rt", "target": "iIzk8fHma58K", "amount": 922.28, "currency": "USD"}
{"source": "pNdyWUR6RqVJ", "target": "iALP36n0pMa6", "amount": 933.16, "currency": "USD"}
{"source": "YNtVnaD6swid", "target": "SL1jW08sCITn", "amount": 965.56, "currency": "USD"}