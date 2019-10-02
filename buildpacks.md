
List of all buildpack commands: 
    
        cf --help -a |grep -i buildpack

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

How do I update the buildpack with the new version?
    
    $ cf update-buildpack go_buildpack -p https://github.com/cloudfoundry/go-buildpack/releases/download/v1.8.11/go-buildpack-v1.8.11.zip 

How do I lock a buildpack to prevent updates?
Lock a buildpack if your application cannot be updated to a newer version.

    $ cf update-buildpack some-buildpack-name --lock

How do I unlock a buildpack to allow updates?

    $ cf update-buildpack some-buildpack-name --unlock

How do I rename a buildpack?

    $ cf rename-buildpack some-buildpack-name some-new-buildpack-name

How do I delete a buildpack?

    $ cf delete-buildpack some-buildpack-name
    
    
List of system buidpacks:
https://docs.cloudfoundry.org/buildpacks/system-buildpacks.html

List of community buidpacks:
https://github.com/cloudfoundry-community/cf-docs-contrib/wiki/Buildpacks#community-created

Creating a custom buildpack: 
https://docs.cloudfoundry.org/buildpacks/custom.html


