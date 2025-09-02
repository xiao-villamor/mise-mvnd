# mise-mvnd

A modified version of the official [mise-maven](https://github.com/mise-plugins/mise-maven) plugin, providing support for the [Apache Maven Daemon (mvnd)](https://maven.apache.org/tools/mvnd.html) within [mise](https://github.com/jdx/mise).

After installing [mise](https://github.com/jdx/mise),
you can install this plugin by running the following command:


```bash
mise plugin install mvnd https://github.com/xiao-villamor/mise-mvnd.git
```

You can then install a default version of maven like this:

```bash
mise use -g mvnd:mvnd@1.0.2
```

The above command will instruct mise-mvnd to always use the latest version of
Maven 1.0.2 by default.

## Using specific Maven versions

You can install a specific version of Maven Daemon like this:

```bash
mise install mvnd:mvnd@1.0.2
```

and switch versions like this:

```bash
mise use mvnd:mvnd@1.0.2
```

This will create a new entry in the .mise.toml file at your repository's root.

### Adding dependencies

Any runtime dependencies required by mise-maven to operate correctly when
used by an end-user should be directly bundled into the source code.
Dependencies used for development or testing purposes only may be added
as git submodules or configured through mise.

## License

All contributions are licensed under the Apache License, Version 2.0
(the "License"); you may not use this file except in compliance with the
License. You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

