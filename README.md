# Nuvent Modules

Standardized modules for the Nuvent declarative cloud infrastructure manager.

## Repository Structure

- `gcp/`: Google Cloud Platform resource modules.
- `github/`: GitHub resource modules.

Each module directory contains a `module.nv` file which defines the variables, resources, and outputs for that module.

## Usage

Modules can be imported into your Nuvent manifest:

```yaml
modules:
  my-bucket:
    source: "github.com/solaegis/nuvent-modules//gcp/storage/bucket"
    variables:
      name: "my-unique-bucket"
      location: "US"
```

## Contributing

1. Ensure all `module.nv` files use the standard schema header.
2. Run `task lint` to validate your changes.
3. Follow the project stewardship model for AGPL-3.0 and CLA compliance.
