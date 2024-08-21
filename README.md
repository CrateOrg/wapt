# wapt (webapt)

### Install .deb packages on systems that don't have apt.

Will install/extract packages to ~/.local/share/wapt/installed .  
Ansible roles and collections are symlinked to ~/.ansible .  
Actions are 'update', 'install' or 'list'.  
Works without root.  
Only dependencies are wget, ar, tar and md5sum.  
Currently not possible to install a specific version of a package.

```
Usage:
  wapt <ACTION> <PACKAGE_NAME> <REPO_URL>
or:
  export WAPT_REPO_URL=<REPO_URL>
  wapt <ACTION> <PACKAGE_NAME>
Example:
  wapt install hello-world http://example.com/repo
  wapt list http://example.com/repo  
```
