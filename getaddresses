import csv

def get_urls(filename='list.csv'):
    start_urls = []
    #df = pd.read_csv(filename).values  # Get only useful stuff
    df = []
    with open(filename, 'r') as csvFile:
        reader = csv.reader(csvFile)
        for row in reader:
            df.append(row)

    csvFile.close()
    for i in df:
        start_urls.append('https://www.whitepages.com.au/residential/results?name={}&location={}, {}&address={}'.format(i[1], i[3], i[4], i[2]))
    return start_urls

data = get_urls('F:/Python/whitepages-scraper/list.csv')
print('data: ', data)
