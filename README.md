# Home Assistant AMOLED Themes
[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=for-the-badge)](https://github.com/hacs/integration)

## All Credits go to JuanMTech for creating the Blue Base... Please consider buying him a coffee! https://github.com/JuanMTech/amoled_blue

### A couple of black-ish Home Assistant themes for devices with AMOLED displays

##### Screenshots
**1. Desktop**
<p align="center">
> Placeholder
</p>

**2. Mobile**
<p align="center">
> Placeholder
</p>

#### Preparation
1. Make sure that under the **configuration.yaml** file you have the following:

<pre>
frontend:
  themes: !include_dir_merge_named themes
</pre>

2. Under the Home Assistant **Config** folder, create a new folder named **themes**
3. **Restart** Home assistant to apply the changes. 

#### HACS installation
1. Go into the Community Store (HACS)
2. Search for Google Dark Theme
3. Open the theme
4. Press Install
5. Restart Home Assistant

#### Manual installation
1. In the Home assistant **themes** folder, create a file named `amoled_blue.yaml`
2. In this GitHub repo, go into the **themes** folder, open the `amoled_blue.yaml` file and copy the content
3. Paste the content in the `amoled_blue.yaml` file created under your Home Assistant themes folder

#### Enable theme
1. Open your Home Assistant **Profile**
2. Under, **Themes**, select the new AMOLED Blue Theme


#### Custom Header settings
When using the [Custom Header](https://github.com/maykar/custom-header) plugin, add the following to make sure that the header matches the theme.

<pre>
custom_header:
  compact_mode: true
  background: var(--app-header-background-color)
  elements_color: var(--app-header-text-color)
  active_tab_color: var(--state-icon-active-color)
  tab_indicator_color: var(--state-icon-active-color)
</pre>

