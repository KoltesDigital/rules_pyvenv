# Bazel rules for creating Python virtual environments

See `example/` for an example.

## Installation

Add the following to your `MODULE.bazel`.

(Note: see the releases page for release-specific `MODULE.bazel` config)

```python
bazel_dep(name = "rules_pyvenv")
```

On Windows, [you need to enable symlink support](https://bazel.build/configure/windows#symlink).

## Example

```bash
cd example
bazel run //:venv myenv
. myenv/bin/activate
```
