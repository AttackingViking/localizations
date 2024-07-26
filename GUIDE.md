# TRMNL localizations guide
overview of our web application interface for higher context translations.

## content hierarchy
the YML file structure (make a copy of `locales/en.yml`) follows a resource-based hierarchy. content on the Account page (`/account`) is thus nested as follows:

```
account:
  index:
    title: Account
    tagline: Manage your account settings
```

if a given phrase is used in other locations, it will be placed in the "root" node of the YML file as global variable:

```
en:
  add: Add
  back: Back
  cancel: Cancel
```

## how to use this guide
below are screenshots of the web app interface with inline annotations to provide the context of each phrase. please note the punctuation, capitalization, and tone as you provide translations. for example, "Edit" is usually text embedded inside a button. it should not, therefore, be written as "edit" or "EDIT."

we understand only some languages support casing. we also understand some languages (ex: Korean) support levels of formality. and finally there are languages with gendered nouns, from Spanish to German. in general we prefer a casual tone with simple vocabularly. this matches the spirit of our brand and makes TRMNL comfortable to use for people all around the world.

## localizations by interface
assuming you've made a copy of the `locales/en.yml` file and replaced `en:` (file, Line 1) with [your language code](https://github.com/ladjs/i18n-locales), let's begin!

#### login
accessible at `/login`.

![login view](/../master/support/login.png?raw=true "login view")

#### signup / register
accessible at `/signup`.

![signup view](/../master/support/signup.png?raw=true "signup view")

#### dashboard
accessible at `/dashboard` while logged in.

![dashboard view](/../master/support/dashboard.png?raw=true "dashboard view")

#### plugins
accessible at `/plugins` while logged in.

![plugins view](/../master/support/plugins.png?raw=true "plugins view")

#### plugin settings (list)
accessible at `/plugin_settings?keyname={{plugin}}` while logged in.

![plugin settings list view](/../master/support/plugin_settings_list.png?raw=true "plugin settings list view")

#### plugin settings (form)
accessible at `/plugin_settings/:id/edit` while logged in.

![plugin settings form view](/../master/support/plugin_settings_form.png?raw=true "plugin settings form view")

#### devices (list)
accessible at `/devices` while logged in.

![devices list view](/../master/support/devices_list.png?raw=true "devices list view")

#### devices (add new)
accessible at `/devices` while logged in, click Add new.

![add device](/../master/support/devices_add.png?raw=true "add new device view")

#### devices (form)
accessible at `/devices/:id/edit` while logged in.

![devices form view](/../master/support/devices_form.png?raw=true "devices form view")

#### playlists
accessible at `/playlists` while logged in.

![playlists view](/../master/support/playlists.png?raw=true "playlists view")

#### account
accessible at `/account` while logged in.

![account view](/../master/support/account.png?raw=true "account view")
