NOTE: Airship has moved away from TSLint and now uses [`typescript-eslint`](https://typescript-eslint.io/) as our primary TypeScript linting tool. This decision was made after reading [The future of TypeScript on ESLint](https://eslint.org/blog/2019/01/future-typescript-eslint) and these lines from the [TypeScript Roadmap](https://github.com/Microsoft/TypeScript/issues/29288)
> we noticed that there were a few architectural issues with the way TSLint rules operate that impacted performance  
> [...]  
> Given this, our editor team will be focusing on leveraging ESLint

With this, Pull Requests are appreciated but our team will be focusing our efforts elsewhere at this time.

# Airship TSLint React a11y Extension

[![npm package](https://img.shields.io/npm/v/@airship/tslint-react-a11y.svg?style=flat-square)](https://www.npmjs.org/package/@airship/tslint-react-a11y)

JSX a11y rules to extend [TSLint](https://palantir.github.io/tslint/) used by the [Airship](https://teamairship.com) Builders. This package is designed to extend the functionality of [@teamairship/tslint-react-config](https://www.npmjs.com/package/@airship/tslint-react-config) while leaving the flexibility to leave these rules out when needed.

## Installation

`yarn add -D @airship/tslint-react-a11y`

## Usage

In `tslint.json`

```js
{
  "extends": ["@airship/tslint-react-a11y"],
    "rules": {
    // override tslint-react-a11y rules here
    "react-a11y-lang": false
  }
}
```

## Supported Rules

All rules are enabled by default.

| Rule Name                                 | Description    |
| :---------------------------------------- | :------------- |
| `react-a11y-accessible-headings`          | There should be no more than 2 H1 heading elements, HTML heading elements must be concise, shouldn't increase by more then one level consecutively and non-empty. |
| `react-a11y-anchors`                      | Anchor elements must have a href different from # and a text longer than 4. |
| `react-a11y-aria-unsupported-elements`    | Enforce that elements that do not support ARIA roles, states, and properties do not have those attributes. |
| `react-a11y-event-has-role`               | Elements with event handlers must have role attribute. |
| `react-a11y-iframes`                      | Enforce that iframe elements are not empty, have title, and are unique. |
| `react-a11y-image-button-has-alt`         | Enforce that inputs element with type="image" must have alt attribute. |
| `react-a11y-img-has-alt`                  | Enforce that an img element contains the non-empty alt attribute. For decorative images, using empty alt attribute and role="presentation". |
| `react-a11y-input-elements`               | HTML input boxes and text areas must include default, place-holding characters. |
| `react-a11y-lang`                         | `html` elements must have a valid lang attribute. |
| `react-a11y-meta`                         | HTML meta elements must not have http-equiv="refresh". |
| `react-a11y-no-onchange`                  | Enforce usage of onBlur over onChange on select menus. |
| `react-a11y-props`                        | Enforce all `aria-*` attributes are valid. Elements cannot use an invalid `aria-*` attribute. |
| `react-a11y-proptypes`                    | Enforce ARIA state and property values are valid. |
| `react-a11y-required`                     | Enforce that required input elements must have aria-required set to true. |
| `react-a11y-role`                         | Elements with aria roles must have all required attributes according to the role. |
| `react-a11y-role-has-required-aria-props` | Elements with aria roles must use a **valid**, **non-abstract** aria role. A reference to role definitions can be found at [WAI-ARIA roles](https://www.w3.org/TR/wai-aria-1.1/#role_definitions). |
| `react-a11y-role-supports-aria-props`     | Enforce that elements with explicit or implicit roles defined contain only `aria-*` properties supported by that `role`. Many aria attributes (states and properties) can only be used on elements with particular roles. Some elements have implicit roles, such as `<a href='hrefValue' />`, which will be resolved to `role='link'`. A reference for the implicit roles can be found at [Default Implicit ARIA Semantics](https://www.w3.org/TR/html-aria/#sec-strong-native-semantics). |
| `react-a11y-tabindex-no-positive`         | Enforce tabindex value is **not greater than zero**. |
| `react-a11y-titles`                       | HTML title elements must be concise and non-empty. |

## Contributing

Bug reports and pull requests are welcome on GitHub at [https://github.com/teamairship/tslint-react-a11y](https://github.com/teamairship/tslint-react-a11y). This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the Contributor Covenant code of conduct.

## License

This package is available as open source under the terms of the [MIT License](https://github.com/teamairship/tslint-react-a11y/blob/master/LICENSE).

## Thanks

- [tslint-react-a11y](https://github.com/joaovieira/tslint-react-a11y) for the inspiration
- [tslint-microsoft-contrib](https://github.com/Microsoft/tslint-microsoft-contrib) for the rules
