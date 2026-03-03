# RoveIQ QGIS Plugin Repository

Custom QGIS plugin repository for the RoveIQ team.

## Setup (One-time)

1. Open QGIS
2. Go to **Plugins → Manage and Install Plugins → Settings** tab
3. Click **Add...** to add a new repository
4. Enter:
   - **Name:** `RoveIQ`
   - **URL:** `https://russellmiddleton33.github.io/roveiqgis-repo/plugins/plugins.xml`
5. Click **OK**
6. Go to the **All** tab → search **RoveiQgis** → click **Install**

## Updating

After initial setup, updates appear automatically in the **Upgradeable** tab of the Plugin Manager. QGIS checks for updates on startup.

## For Developers

This repo is automatically updated by CI when a new version is tagged in the source repository. Do not edit the `plugins/` directory manually.

### Release workflow

```bash
# In the roveiq-gis source repo:
# 1. Bump version in metadata.txt
# 2. Commit
git commit -am "Bump version to X.XX"
# 3. Tag and push
git tag vX.XX
git push origin main --tags
# CI handles the rest
```
