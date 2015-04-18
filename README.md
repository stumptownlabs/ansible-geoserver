# ansible-geoserver

An Ansible role for installing Geoserver 2.7.0 on Ubuntu.

## Role Variables

- `geoserver_version_major` - Geoserver major version (default: `2`)
- `geoserver_version_minor` - Geoserver minor version (default: `7`)
- `geoserver_version_patch` - Geoserver version patch (default: `0`)
- `geoserver_mirror` - Geoserver Sourceforge Download Mirror (default: `http://sourceforge.net/projects/geoserver/files/GeoServer`)
- `geoserver_redis_sha256sum` - Sha256sum for Geoserver 2.7.0 war file (default: `9d5c52e1137c6393cee17679b88eee2d728842a7449da004cecb805da8fc8f1a`)
- `ansible_data_path` - Download directory for Geoserver war file (default: `/home/vagrant`)

## Dependencies

- Requires Apache Tomact 7 installed at `/var/lib/tomcat7/`


## Example Playbook

    - hosts: servers
      roles:
         - { role: stumptownlabs.geoserver }

## License

Apache2
