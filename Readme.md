# Quebec Municipalities Scraper

This is a web scraper built with Scrapy. It scrapes data from the Quebec government's directory of municipalities.

## Installation

Before running the scraper, you need to install the required Python packages. You can do this by running the following command in your terminal:

```bash
pip install -r requirements.txt
```
This will install all the necessary packages listed in the requirements.txt file.

## Usage

To run the scraper, use the following command:

```bash
scrapy runspider quotes_scraper/quotes_scraper/spiders/quotes_spider.py
```

This will run the scraper and save the output to a file named output.csv. You can change the output file name to whatever you like.
If you want to save the output to a different format, you can change the file extension to .json or .xml.

```
scrapy runspider quotes_scraper/quotes_scraper/spiders/quotes_spider.py -o quotes.json
```

This will save the output to a file named quotes.json. You can also save the output to a .xml file by changing the file extension to .xml.

```
scrapy runspider quotes_scraper/quotes_scraper/spiders/quotes_spider.py -o quotes.xml
```

## Spider Details

The spider starts at the URL defined in start_urls and extracts the data defined in the parse method. It follows the link to the next page, repeating the process until there are no more pages.

The data extracted includes the name of the municipality, the type of municipality, the region, the population, and the area.

* Quote text
* Author name
* Tags

These are extracted from div elements with the class quote on the page. The spider uses CSS selectors to select these elements and extract the data.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```
Please replace the placeholder text with the actual details of your project.
```
