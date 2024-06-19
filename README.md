## Hi there 👋

<!--
**Latisha19/Latisha19** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

<!--START_SECTION:waka-->
name: Waka Readme

on:
schedule:
    - cron: '0 0 * * *'
workflow_dispatch:
jobs:
update-readme:
    name: Update Readme with Metrics
    runs-on: ubuntu-latest
    steps:
    - uses: anmol098/waka-readme-stats@master
        with:
        WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
        GH_TOKEN: ${{ secrets.GH_TOKEN }}
        SHOW_PROFILE_VIEWS: False
        <!--SHOW_SHORT_INFO: False
        SHOW_LOC_CHART: False-->
        SHOW_PROJECTS: False

<!--END_SECTION:waka-->
