# Shaarli Image Upload Plugin

This plugin for Shaarli allows users to upload an image file when sharing a link. The image is stored in the `data/images` directory, and a link to the image is automatically prefilled in the text content dialog.

## Features

- Image upload when sharing a link: When you share a link, you can select and upload an image file from your computer. The image file is then stored on the server.
- Automatic link to the image: After the image is uploaded, a link to the image is automatically added to the text content of the shared link. This makes it easy to include a relevant image with each link you share.
- Easy integration: The plugin is designed to integrate seamlessly with Shaarli's existing features and plugins. It does not require any changes to your Shaarli installation, and can be enabled or disabled from the plugin administration page.

## Installation

To install the plugin, download the latest release and extract it to the `plugins` directory of your Shaarli installation. Then, go to the plugin administration page and enable the Image Upload plugin.

### Docker Installation

If you're running Shaarli in a Docker container, you can use a Docker volume to install the plugin:

1. First, download the plugin and save it to a directory on your host machine, e.g., `/path/to/your/plugins/image_upload`.

2. Then, when starting your Shaarli Docker container, mount the directory to the correct path inside the container with the `-v` option:

```bash
docker run -v /path/to/your/plugins/image_upload:/var/www/shaarli/plugins/image_upload -d -p 80:80 --name shaarli shaarli/shaarli
```

This command will start a new Shaarli container and make the Image Upload plugin available in the `plugins` directory of your Shaarli installation.

## Usage

When you share a link, you will see an option to upload an image. Click the "Choose File" button, select an image file, and then click "Save". The image will be uploaded to the server, and a link to the image will be added to the text content of the shared link.

## Contributing

Contributions to the plugin are welcome. If you find a bug or have an idea for a new feature, please open an issue or submit a pull request.
