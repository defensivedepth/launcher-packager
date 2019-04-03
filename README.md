# launcher-packager
One-shot container that generates customized Launcher osquery packages.



Usage:   
`docker run \`   
`--mount type=bind,source="$(pwd)",target=/output \`   
 `defensivedepth/launcher-packager:latest "$EnrollSecret" "$FleetHostname" "$AutoUpdate(enabled|disabled)"`   

The last option is for whether or not the Autoupdate flag should be set. If `enabled`, then autoupdate will be enabled and the `stable` channel will be used.

The packages will be copied out to your current directory.
