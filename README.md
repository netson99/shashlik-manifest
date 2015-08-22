## shashlik-manifest
This project is a source code manifest for all projects currently used by shashlik.
It is used by Android `repo` tool to automatically download all projects that are needed by shashlik.

### Prepare
If you alredy have Android `repo` available on your system, sync your code as shown in **Download** section below.

1. Make sure you have a bin/ directory in your home directory and that it is included in your path:

  ```
  $ mkdir ~/bin
  $ PATH=~/bin:$PATH
  ```
  
2. Download the Repo tool and ensure that it is executable:

  ```
  $ curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
  $ chmod a+x ~/bin/repo
  ```

### Download
Invoke this `repo` command to get all projects that are required by shashlik in one go!

  ```
  $ mkdir shashlik
  $ cd shashlik
  $ repo init -u git@github.com:darkenk/shashlik-manifest.git -b shashlik-5.1.1_r9
  ```
  
If everything goes well, you should end up with source code in your current directory.
