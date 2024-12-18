# Uploading a Plugin Manifest JSON File

This document provides step-by-step instructions for users to upload a `manifest.json` file to integrate a plugin with Weave.

## Prerequisites

1. Ensure you have a valid `manifest.json` file. Below is an example structure:

   ```json
   {
     "id": "callback-data-plugin",
     "name": "Callback Data",
     "description": "Callback Data integration for Weave",
     "image": "http://example.com/callback-data.png",
     "version": "1.0.0",
     "repo": "http://github.com/xyz/callback-data",
     "type": "page",
     "src": "http://localhost:8888/calls"
   }
   ```

2. Verify the following:
   - The `id` is unique for your plugin.
   - The `image` URL points to an accessible resource.
   - The `src` URL is functional and points to the plugin’s endpoint.

## Steps to Upload the Manifest

### Step 1: Access the Weave Plugin Management Page

1. Log in to your Weave admin portal.
2. Navigate to the **Plugin Management** section. This can usually be found under **Settings** > **Plugins**.

### Step 2: Upload the `manifest.json` File

1. Click the **Upload Plugin** button.
2. In the upload dialog box:
   - Select the `manifest.json` file from your computer.
   - Click **Open** to confirm the selection.

### Step 3: Verify the Plugin Information

1. After uploading, Weave will parse the `manifest.json` and display the plugin details, including:

   - Plugin name
   - Description
   - Version
   - Image preview (if provided)

2. Review the information to ensure correctness.

### Step 4: Confirm and Activate

1. Click **Confirm Upload** to proceed.
2. The plugin will now appear in the plugin list. Locate your plugin and toggle the **Activate** switch to enable it.

## Troubleshooting

1. **Error: Invalid JSON Format**

   - Verify that your `manifest.json` file is properly formatted. Use a JSON validator tool if needed.

2. **Error: Missing Fields**

   - Ensure all required fields (`id`, `name`, `description`, `version`, `type`, and `src`) are included and populated.

3. **Error: Inaccessible Resources**
   - Confirm that the `image` and `src` URLs are publicly accessible and not restricted by a firewall.

## Additional Notes

- **Local Development:** For local development, ensure your `src` URL (e.g., `http://localhost:8888/calls`) is accessible from the machine hosting the Weave platform.
- **Versioning:** Update the `version` field if you make changes to the plugin and re-upload the manifest.
- **Repository URL:** Providing a `repo` URL is optional but recommended for tracking and collaboration.

Following these steps will ensure a seamless process for uploading and activating your plugin’s manifest file.
