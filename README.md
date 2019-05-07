# ![LOGO](logo.png) CircleCI **flow**ground Connector

## Description

A generated **flow**ground connector for the CircleCI API (version v1).

Generated from: https://api.apis.guru/v2/specs/circleci.com/v1/swagger.json<br/>
Generated at: 2019-05-07T17:39:56+03:00

## API Description

The CircleCI API is a RESTful, fully-featured API that allows you to do almost anything in CircleCI.
You can access all information and trigger all actions.
The only thing we don’t provide access to is billing functions, which must be done from the CircleCI web UI.


## Authorization

Supported authorization schemes:
- API Key
## Actions

### Provides information about the signed in user.

### Build summary for each of the last 30 builds for a single git repo.

#### Input Parameters
* `limit` - _optional_ - The number of builds to return. Maximum 100, defaults to 30.

* `offset` - _optional_ - The API returns builds starting from this offset, defaults to 0.

* `filter` - _optional_ - Restricts which builds are returned.
Set to "completed", "successful", "failed", "running", or defaults to no filter.

    Possible values: completed, successful, failed, running.

### Triggers a new build, returns a summary of the build.

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX


### Clears the cache for a project.

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX


### Lists checkout keys.

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX


### Creates a new checkout key.<br/>
> Only usable with a user API token.

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX


### Delete a checkout key.

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX

* `fingerprint` - _required_ - XXXXXXXXXX


### Get a checkout key.

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX

* `fingerprint` - _required_ - XXXXXXXXXX


### Lists the environment variables for :project

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX


### Creates a new environment variable

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX


### Deletes the environment variable named ':name'

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX

* `name` - _required_ - XXXXXXXXXX


### Gets the hidden value of environment variable :name

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX

* `name` - _required_ - XXXXXXXXXX


### Create an ssh key used to access external systems that require SSH key-based authentication

#### Input Parameters
* `Content-Type` - _required_
    Possible values: application/json.
* `project` - _required_ - XXXXXXXXX


### Triggers a new build, returns a summary of the build.<br/>
> Optional build parameters can be set using an experimental API.<br/>
> <br/>
> Note: For more about build parameters, read about [using parameterized builds](https://circleci.com/docs/parameterized-builds/)

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX

* `branch` - _required_ - The branch name should be url-encoded.


### Full details for a single build. The response includes all of the fields from the build summary.<br/>
> This is also the payload for the [notification webhooks](/docs/configuration/#notify), in which case this object is the value to a key named 'payload'.

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX

* `build_num` - _required_ - XXXXXXXXXX


### List the artifacts produced by a given build.

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX

* `build_num` - _required_ - XXXXXXXXXX


### Cancels the build, returns a summary of the build.

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX

* `build_num` - _required_ - XXXXXXXXXX


### Retries the build, returns a summary of the new build.

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX

* `build_num` - _required_ - XXXXXXXXXX


### Provides test metadata for a build<br/>
> Note: [Learn how to set up your builds to collect test metadata](https://circleci.com/docs/test-metadata/)

#### Input Parameters
* `username` - _required_ - XXXXXXXXX

* `project` - _required_ - XXXXXXXXX

* `build_num` - _required_ - XXXXXXXXXX


### List of all the projects you're following on CircleCI, with build information organized by branch.

### Build summary for each of the last 30 recent builds, ordered by build_num.

#### Input Parameters
* `limit` - _optional_ - The number of builds to return. Maximum 100, defaults to 30.

* `offset` - _optional_ - The API returns builds starting from this offset, defaults to 0.


### Adds your Heroku API key to CircleCI, takes apikey as form param name.

## License

**flow**ground :- Telekom iPaaS / circleci-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
