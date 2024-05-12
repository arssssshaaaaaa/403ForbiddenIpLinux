# Hello This Tool Help You To Fix Your Package Installer In Kali Linux terminal With This Error W: Failed to fetch http://old-releases.ubuntu.com/ubuntu/dists/saucy-security/universe/binary-i386/Packages 403 Forbidden

So For Fix This You Need Download The Source-List File Inside With Simples Levels

# Cloning

Open Your Terminal And Type This Commands

1- `git clone https://github.com/arssssshaaaaaa/403ForbiddenIpLinux`

2- `cd 403ForbiddenIpLinux `

3- `sudo mv source.list /etc/apt `
Again run the `sudo apt-get update ` And You See New Error Like This

Get:1 http://security.ubuntu.com/ubuntu xenial-security InRelease [99.8 kB]
Err:1 http://security.ubuntu.com/ubuntu xenial-security InRelease
The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 40976EAF437D05B5 NO_PUBKEY 3B4FE6ACC0B21F32
Get:2 http://us.archive.ubuntu.com/ubuntu xenial InRelease [247 kB]  
Err:2 http://us.archive.ubuntu.com/ubuntu xenial InRelease
The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 40976EAF437D05B5 NO_PUBKEY 3B4FE6ACC0B21F32
Get:3 http://us.archive.ubuntu.com/ubuntu xenial-updates InRelease [99.8 kB]
Err:3 http://us.archive.ubuntu.com/ubuntu xenial-updates InRelease  
 The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 40976EAF437D05B5 NO_PUBKEY 3B4FE6ACC0B21F32
Get:4 http://us.archive.ubuntu.com/ubuntu xenial-backports InRelease [97.4 kB]
Err:4 http://us.archive.ubuntu.com/ubuntu xenial-backports InRelease  
 The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 40976EAF437D05B5 NO_PUBKEY 3B4FE6ACC0B21F32
Reading package lists... Done  
W: GPG error: http://security.ubuntu.com/ubuntu xenial-security InRelease: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 40976EAF437D05B5 NO_PUBKEY 3B4FE6ACC0B21F32
E: The repository 'http://security.ubuntu.com/ubuntu xenial-security InRelease' is not signed.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.
W: GPG error: http://us.archive.ubuntu.com/ubuntu xenial InRelease: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 40976EAF437D05B5 NO_PUBKEY 3B4FE6ACC0B21F32
E: The repository 'http://us.archive.ubuntu.com/ubuntu xenial InRelease' is not signed.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.
W: GPG error: http://us.archive.ubuntu.com/ubuntu xenial-updates InRelease: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 40976EAF437D05B5 NO_PUBKEY 3B4FE6ACC0B21F32
E: The repository 'http://us.archive.ubuntu.com/ubuntu xenial-updates InRelease' is not signed.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.
W: GPG error: http://us.archive.ubuntu.com/ubuntu xenial-backports InRelease: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 40976EAF437D05B5 NO_PUBKEY 3B4FE6ACC0B21F32
E: The repository 'http://us.archive.ubuntu.com/ubuntu xenial-backports InRelease' is not signed.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.

For Fix This You Need Generate a New Public Key

# Create New Public Key

For Generate a New Public This Command

` sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 40976EAF437D05B5`

our this

`sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 3B4FE6ACC0B21F32 `

And You See Your Package Is Installing :)
