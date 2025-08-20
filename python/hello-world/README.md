# hello world pipeline example in Python

A simple RDF-Connect pipeline example with Python processors.

We lock the Python version to 3.13.* in the `pyproject.toml` file such that we can have a deterministic path where our packages are installed.
We need this path to be able to `owl:imports` the Python runner and processor packages in the RDF-Connect pipeline configuration.

## Usage

### Install Dependencies

#### Node

Install the Node.js dependencies:

```shell
npm install
```

#### Python

Install the Python dependencies:

```shell
hatch env create
hatch shell
```

### Run the Pipeline

Run the pipeline using the `rdfc` command:

```shell
rdfc pipeline.ttl
```
