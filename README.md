
# Zoe Depth Estimation

This is an end-to-end python api project.


## Usage/Examples

### CLI USAGE
```bash
usage: cli.py [-h] input_image output_image

Depth estimator with using ZoeDepth

positional arguments:
  input_image   Path to input image
  output_image  Path to output depthmap

options:
  -h, --help    show this help message and exit
```

### API USAGE
```
http://127.0.0.1:8041/predict
```

## Installation

Install depth estimation project with pip

```bash
  pip install -r requirements.txt
```
    
## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`IMG_API_KEY` from `https://imgbb.com/api`


## Deployment

To deploy this project run

```bash
  docker build -t depth_estimation . 
  docker run -d -p 8041:8041 depth_estimation  
```


## License

[MIT](https://choosealicense.com/licenses/mit/)

