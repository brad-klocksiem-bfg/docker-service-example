# Getting Started

This is a standard nginx, django powered service running under Docker containers.  The services are configured via configuration files supplied at build time.  These files can be tuned to enhance functionality, and free resources.  As a starter, clone this repository and tweak the settings to your desire.  The configuration file supplied looks like this:

```yaml
debug: true
fun-factor: enhanced
maintainers: ['john.doe@fakeorg.com', 'jane.doe@fakeorg.com']
```

Once ready, run the included build script and magic will take care of the rest.

# Usage Examples

Additionally, you can try out the following other settings:

## Basic

```yaml
debug: true
```

## Advanced

```yaml
debug: true
fun-factor: extreme
maintainers: ['john.doe@fakeorg.com', 'jane.doe@fakeorg.com']
mysql: deprecated
memcruncher: enabled
knuthian-accelerators: enabled
```