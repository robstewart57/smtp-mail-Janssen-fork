# CHANGELOG

This package follows the Package Versioning Policy.
Roughly speaking, this means that we have four digits standing for:

- Major: A significant rewrite of the library.
- Major: A breaking change
- Minor: A non-breaking addition
- Patch: A non-breaking bugfix

## Upcoming

If you are doing a pull-request, please update this list.
A template is provided:

```
- [# PR number](URL to pr) @your_github_username
  - Describe change #1
  - Describe change #2
  - Indicate if changes are major, minor, or patch changes.
```

## 0.4.0.2

- Switch to `crypton` because the `cryptonite` package is no longer maintained.

## 0.4.0.1

- [#11](https://github.com/haskell-github-trust/smtp-mail/pull/11) @spencerjanssen
    - Support `crypton-connection-0.4.0`

## 0.4.0.0

- [#5](https://github.com/haskell-github-trust/smtp-mail/pull/5) @spencerjanssen
    - Switch to `crypton-connection` because the `connection` package is no longer maintained
- [#6](https://github.com/haskell-github-trust/smtp-mail/pull/6) @spencerjanssen
    - [Change in maintainership](https://github.com/jhickner/smtp-mail/pull/41#issuecomment-2012521041)

## 0.3.0.0

- [#32](https://github.com/jhickner/smtp-mail/pull/32) @typetetris
    - add some functions to use SMTPS, which should be preferred to
      STARTTLS for mail submissions of endusers according to RFC 8314
    - add STARTTLS
    - add integration test using nixos tests

- [#30](https://github.com/jhickner/smtp-mail/pull/30) @typetetris
    - Replace `cryptohash` dependency with `cryptonite`.
      `cryptohash` is deprecated and `cryptonite` offers HMAC MD5
      directly.

## 0.2.0.0

- [#25](https://github.com/jhickner/smtp-mail/pull/25) @shulhi
    - References to the deprecated `Network` module were removed and replaced 
      with the new `connection` package. 
    - Duplicate functionality was deprecated.
- [#23](https://github.com/jhickner/smtp-mail/pull/23) @alexandersgreen
    - The `Cc` and `Bcc` fields will be sent to the SMTP server, and they'll 
      actually be sent now. 
