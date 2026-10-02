# Kid Garden / Picture Garden

Public website for Kid Garden and its children's mobile app, Picture Garden.

## GitHub Pages

In the repository settings, open **Pages** and select **Deploy from a branch**, then choose the `main` branch and `/ (root)`. GitHub Pages processes the Jekyll permalinks declared in each page's front matter.

## Local preview

The extensionless page links require a web server that processes the Jekyll permalinks; opening the HTML files directly with `file://` will not work. To preview locally with the same GitHub Pages-compatible Jekyll version:

1. Install Ruby and Bundler. On Windows, RubyInstaller with the MSYS2 development toolchain is a suitable option.
2. From the repository root, install the dependencies:

	```sh
	bundle install
	```

3. Start Jekyll:

	```sh
	bundle exec jekyll serve
	```

4. Open `http://127.0.0.1:4000/`. The local routes match production: `/privacy/`, `/team/`, and `/picture-garden/`.

## Before publishing

Before submitting the privacy page to Google Play, confirm the contact address is monitored and verify every statement against the released app and all SDKs/services it uses.

Confirm and document:

- The privacy contact address is monitored and reaches the app operator.
- Whether any included SDK or third-party service collects or receives data contrary to the statements in the policy.
- The app's target age groups, advertising status, parent-facing controls, and Google Play declarations.
- Confirmation that purchase handling and any information returned to the app match the description of Google Play billing.
- Consistency between the final policy, the app, Google Play's target audience/Families declarations, and the Data safety form.

The privacy policy must be publicly accessible, kept current, linked from the app and the relevant Google Play listing, and accurately describe actual behavior. Review Google's current [privacy policy guidance](https://support.google.com/googleplay/android-developer/answer/9859455?hl=en#privacy_policy) and [Families policy](https://support.google.com/googleplay/android-developer/answer/10144311?ref_topic=9877467) before release.
