# consul-snapshot-boshrelease

BOSH release to run [consul-snapshot](https://github.com/pshima/consul-snapshot).

## Usage


To use this bosh release, first upload it to your bosh:

```
bosh upload release https://github.com/hybris/consul-snapshot-boshrelease
```

For [bosh-lite](https://github.com/cloudfoundry/bosh-lite), you can quickly create a deployment manifest & deploy a cluster:

```
templates/make_manifest warden
bosh -n deploy
```

For AWS EC2, create a single VM:

```
templates/make_manifest aws-ec2
bosh -n deploy
```
