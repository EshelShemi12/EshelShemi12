

name: DevCard

on:
  workflow_dispatch:
  push:
    branches:
      - main
  schedule:
    - cron: "0 0 * * *"

jobs:
  devcard:
    runs-on: ubuntu-latest
    steps:
      - name: devcard
        uses: dailydotdev/action-devcard@2.0.2
        with:
          devcard_id: <a href="https://app.daily.dev/Eshel"><img src="https://api.daily.dev/devcards/aa7a93a8db634c38851f81764545fa71.png?r=c7i" width="400" alt="DirePant S's Dev Card"/></a>
