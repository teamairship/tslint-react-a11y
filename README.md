# Airship TSLint React a11y Extension

JSX a11y rules to extend [TSLint](https://palantir.github.io/tslint/) used by the [Airship](https://teamairship.com) Builders. Big thanks to what appears to be a stale [tslint-react-a11y](https://github.com/joaovieira/tslint-react-a11y) for the inspiration and [tslint-microsoft-contrib](https://github.com/Microsoft/tslint-microsoft-contrib) for the rules. This package is designed to extend the functionality of [@teamairship/tslint-react-config](https://github.com/teamairship/tslint-react-config) while leaving the flexibility to leave these rules out when needed.

## Installation

`yarn add -D @airship/tslint-react-a11y`

## Usage

In `tslint.json`

```json
{
  "extends": ["@airship/tslint-react-a11y"]
}
```

## Supported Rules

| Rule Name                                 | Description    |
| :---------------------------------------- | :------------- |
| `react-a11y-accessible-headings`          | Coming soon... |
| `react-a11y-anchors`                      | Coming soon... |
| `react-a11y-aria-unsupported-elements`    | Coming soon... |
| `react-a11y-event-has-role`               | Coming soon... |
| `react-a11y-image-button-has-alt`         | Coming soon... |
| `react-a11y-img-has-alt`                  | Coming soon... |
| `react-a11y-input-elements`               | Coming soon... |
| `react-a11y-lang`                         | Coming soon... |
| `react-a11y-meta`                         | Coming soon... |
| `react-a11y-no-onchange`                  | Coming soon... |
| `react-a11y-props`                        | Coming soon... |
| `react-a11y-proptypes`                    | Coming soon... |
| `react-a11y-required`                     | Coming soon... |
| `react-a11y-role`                         | Coming soon... |
| `react-a11y-role-has-required-aria-props` | Coming soon... |
| `react-a11y-role-supports-aria-props`     | Coming soon... |
| `react-a11y-tabindex-no-positive`         | Coming soon... |
| `react-a11y-titles`                       | Coming soon... |

## Contributing

Bug reports and pull requests are welcome on GitHub at [https://github.com/teamairship/tslint-react-a11y](https://github.com/teamairship/tslint-react-a11y). This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the Contributor Covenant code of conduct.

## License

This package is available as open source under the terms of the [MIT License](https://github.com/teamairship/tslint-react-a11y/blob/master/LICENSE).
