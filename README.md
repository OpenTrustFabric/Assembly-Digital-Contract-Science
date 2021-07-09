<img src="https://secureservercdn.net/160.153.137.210/86v.eb1.myftpupload.com/wp-content/uploads/2020/09/Logos-3.png?time=1625746717" align="right" width="120"/>

# WP3_UseCases

This repository includes a set of analytical notebooks that demonstrate **digital contract science**.

Digital contract science makes use of the digital contracts approach that the Open Trust Fabric community develops and combines data science methods in an attempt to provide insights on digital economy to policy makers and others interested.

The notebooks are implemented in Jupyter by following the literate programming approach that combines documentation, analysis code in Python, refined data, and visualizations that together enable actors with different backgrounds to come together to make sense of digital economy and different applications of digital contract science in it.

To run the all the notebooks, you have to set up the analytical infrastructure and access the source datasets. For Use Case 1, we provide a public dataset that allows running and extending the notebooks and invite you to join us in making sense of the platform economy around Airbnb. For source data, please refer to [Inside Airbnb](http://insideairbnb.com/get-the-data.html).

## Setting up

For easy access to the analytical notebooks, you can use Binder: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OpenTrustFabric/WP3_UseCases/HEAD)

We use Python <code>virtualenv</code> to manage the analytical environment for the three use cases.

The following procedure applies directly to Linux and MacOS. For Windowds, you have to adapt the commands accordingly. Consider installing [Anaconda](https://www.anaconda.com/).

Once you have cloned this repository, create a dedicated virtual environment for your local project:

        python3 -m venv env

Activate the environment:

		source env/bin/activate

Following virtual environment practices, you can install the needed modules and libraries all in one go:

		pip install -r requirements.txt
		
Now we should be ready to fire off Jupyter. Run the server and the analytical environment should open up in your browser:

		jupyter notebook

We use Graphistry as the primary visualization tool. To enable Graphistry:

1. Create an account.
2. Create a copy of config_template.json and name it config.json. 
3. Include Graphistry username and password in config.json. 

For more information about Graphistry and authentication, see  [Running Graphistry & Voilà on Binder](https://github.com/graphistry/pygraphistry/issues/240).
