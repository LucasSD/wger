﻿# wger
<img src="https://raw.githubusercontent.com/wger-project/wger/master/wger/core/static/images/logos/logo.png" width="100" height="100" />

wger (ˈvɛɡɐ) Workout Manager is a free, open source web application that help
you manage your personal workouts, weight and diet plans and can also be used
as a simple gym management utility. It offers a REST API as well, for easy
integration with other projects and tools.

For a live system, refer to the project's site: <https://wger.de/>

![Workout plan](https://raw.githubusercontent.com/wger-project/wger/master/wger/software/static/images/workout.png)


## Mobile app
[<img src="https://play.google.com/intl/en_us/badges/images/generic/en-play-badge.png"
      alt="Get it on Google Play"
      height="80">](https://play.google.com/store/apps/details?id=de.wger.flutter)


## Installation

These are the basic steps to install and run the application locally on a Linux
system. There are more detailed instructions, other deployment options as well
as an administration guide available at <https://wger.readthedocs.io> or locally
in your code repository in the docs folder.

Please consult the commands' help for further information and available
parameters.


### Production

If you want to host your own instance, take a look at the provided docker
compose file. This config will persist your database and uploaded images:

<https://github.com/wger-project/docker>

### Demo

If you just want to try it out:

```shell script
    docker run -ti --name wger.apache --publish 8000:80 wger/apache
```

Then just open <http://localhost:8000> and log in as **admin**, password **adminadmin**

Please note that this image will overwrite your data when you pull a new version,
it is only intended as an easy to setup demo

### Development version

We provide a docker compose file that sets everything up for development and
persists the database on a volume. From the root folder just call

````shell script
docker-compose -f extras/docker/compose/docker-compose.yml up
````

Log in as: **admin**, password **adminadmin**

For more info, check the [README in wger/extras/docker/compose](
 ./extras/docker/compose/README.md
).

#### Local installation

If you prefer a local installation, consult the
[development documentation](https://wger.readthedocs.io/en/latest/development.html)


## Contact

Feel free to contact us if you found this useful or if there was something that
didn't behave as you expected. We can't fix what we don't know about, so please
report liberally. If you're not sure if something is a bug or not, feel free to
file a bug anyway.

* **discord:** <https://discord.gg/rPWFv6W>
* **issue tracker:** <https://github.com/wger-project/wger/issues>
* **twitter:** <https://twitter.com/wger_project>


## Sources

All the code and the content is available on github:

<https://github.com/wger-project/wger>


## Translation
Translate the app to your language on [Weblate](https://hosted.weblate.org/engage/wger/).

[![translation status](https://hosted.weblate.org/widgets/wger/-/web/multi-blue.svg)](https://hosted.weblate.org/engage/wger/)


## License

The application is licensed under the Affero GNU General Public License 3 or
later (AGPL 3+).

The initial exercise and ingredient data is licensed additionally under one of
the Creative Commons licenses, see the individual exercises for more details.

The documentation is released under a CC-BY-SA: either version 4 of the License,
or (at your option) any later version.

Some images were taken from Wikipedia, see the SOURCES file in their respective
folders for more details.
