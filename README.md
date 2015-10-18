# jenkinsci-cookbook

TODO: Enter the cookbook description here.

## Supported Platforms

TODO: List your supported platforms.

## Attributes

<table>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td><tt>['jenkinsci']['bacon']</tt></td>
    <td>Boolean</td>
    <td>whether to include bacon</td>
    <td><tt>true</tt></td>
  </tr>
</table>

## Usage

### Before: Install

``` cmd
vagrant plugin install vagrant-berkshelf
vagrant plugin install vagrant-omnibus
bundle install
```

### Vagrant

``` cmd
bundle exec vagrant up
```

### Kitchen.ci

``` cmd
bundle exec kitchen converge / test
```

### jenkinsci::default

Include `jenkinsci` in your node's `run_list`:

```json
{
  "run_list": [
    "recipe[jenkinsci::default]"
  ]
}
```

## License and Authors

Author:: Juan Carlos Alonso Holmstron (j.carlos.alonso.h@gmail.com)
