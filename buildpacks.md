
How do I see what buildpacks are available on my CF environment?

    $ cf buildpacks

If you would like to use a custom buildpack, such as the Swift Language buildpack, you can pass it on the command line like:

    $ cf push -b https://github.com/cloudfoundry-community/swift-buildpack.git

Or, you can add it as a value in your manifest.yml file:

    buildpack: https://github.com/cloudfoundry-community/swift-buildpack.git

How do I add a buildpack to my CF environment?

    $ cf create-buildpack some-build-pack-name /path/to/buildpack.zip 10

How do I change the position of an existing buildpack?

    $ cf update-buildpack some-buildpack-name -i <new position number>

Lock a buildpack if your application cannot be updated to a newer version.
How do I lock a buildpack to prevent updates?

    $ cf update-buildpack some-buildpack-name --lock

How do I unlock a buildpack to allow updates?

    $ cf update-buildpack some-buildpack-name --unlock

How do I rename a buildpack?

    $ cf rename-buildpack some-buildpack-name some-new-buildpack-name

How do I delete a buildpack?

    $ cf delete-buildpack some-buildpack-name
