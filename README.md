# Elasticsearch Configuration

ES configuration utility for OpenPaaS ESN.

The current package contains:

- Indexes configuration in data folder
- A CLI to create indexes

## Create indexes from CLI

Install the CLI from NPM

``` bash
npm install -g esn-elasticsearch-configuration
```

Then use it

```bash
esn-elasticsearch-configuration index contacts --host 192.168.99.100 --port 9200
```

Will create the contacts index on ES running on 192.168.99.100:9200.
Full help is available 'esn-elasticsearch-configuration --help'

## Releasing

Before pushing to NPM, generate the dist folder:

```
grunt package
```

Then login to npm from the command line and release using grunt release plugin (adapt version number):

```
grunt release:0.3.0
```

## License

AGPL-3.0
