# Zoom Client

A Python client for interfacing with the Zoom API to perform various tasks.

## Requirements and Documentation

* Python >= 3.6: [https://www.python.org/downloads/](https://www.python.org/downloads/)
* Enable Zoom API key: [https://zoom.us/developer/api/credential](https://zoom.us/developer/api/credential)

Zoom API documentation can be found at the following URL: [https://marketplace.zoom.us/docs/api-reference/zoom-api](https://marketplace.zoom.us/docs/api-reference/zoom-api)

## Installation

```shell
pip install git+https://github.com/CUBoulder-OIT/zoom_client@main#egg=zoom_client
```

## Usage

1. Ensure requirements outlined above are completed.
2. Provide necessary &lt;bracketed&gt; areas in examples/sample_config.json specific to your account

## Example
```python
#open config file with api key/secret information
config_file = open(run_path+"/config/config.json")
config_data = json.load(config_file)

#create Zoom python client
zoom = controller.controller(config_data)

zoom.users.get_current_users()
zoom_user_counts = zoom.users.get_current_user_type_counts()
```

## License

MIT - See LICENSE
