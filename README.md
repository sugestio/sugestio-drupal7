# Overview

This reference implementation illustrates how the [Sugestio](http://www.sugestio.com) 
recommendation service can be integrated into Drupal 7. Get personal recommendations and 
similar nodes based on [Fivestar](http://drupal.org/project/fivestar) voting behaviour.  

## About Sugestio

Sugestio is a scalable and fault tolerant service that now brings the power of 
web personalisation to all developers. The RESTful web service provides an easy to use 
interface and a set of developer libraries that enable you to enrich 
your content portals, e-commerce sites and other content-based websites.

### Access credentials and the Sandbox

To access the Sugestio service, you need an account name and a secret key. 
To run the examples from the tutorial, you can use the following credentials:

* account name: <code>sandbox</code>
* secret key: <code>demo</code>

The Sandbox is a *read-only* account. You can use these credentials to experiment 
with the service. The Sandbox can give personal recommendations for users 1 through 5, 
and similar items for items 1 through 5.

When you are ready to work with real data, you may apply for a developer account through 
the [Sugestio website](http://www.sugestio.com).  

## About this module

### Features

The following [API](http://www.sugestio.com/documentation) features are fully implemented:

* get personalized recommendations for a given user
* get nodes that are similar to the current node
* submit user activity (consumptions): fivestar-votes and optional click-tracking
* submit node title and URL through hook_nodeapi

Hooks are provided for the following features:

* submit item metadata: description, location, tags, categories, ...  	
* submit user metadata: gender, location, birthday, ...


### Requirements

This module depends on the [Libraries API](http://drupal.org/project/libraries), 
[Fivestar](http://drupal.org/project/fivestar) and 
[sugestio-php](http://github.com/sugestio/sugestio-php), an external library 
for communicating with the webservice. See INSTALL.txt for detailed instructions.

# License

Reference implementation of a Drupal 7 module for the Sugestio recommendation service

Copyright (C) 2011 Sugestio.com

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation; either version 2
of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.