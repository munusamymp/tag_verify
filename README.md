Data bag and secret file setup
The test-kitchen initialization should create a test/integration/default directory. As of test-kitchen pull request #124, cookbook files are aggressively filtered from being copied to the chef-solo working directory. Adding these files to the suite section of the .kitchen.yml will ensure those files get copied over for your integration testing.

First, create a throwaway secret to encrypt testing data.
