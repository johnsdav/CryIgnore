# CryIgnore
Repository contains sample `.gitignore` and `.gitattribute` files for managing a game
module in CryEngine with git.

### Getting Started
1. Copy `.gitignore` and `.gitattribute` into your git project directory

### Package/Build Files
These files include any resources created by the resource compiler which are next text based. Examples include compiled
texture files, animation files and databases, and compressed archives.

```text
*.caf filter=lfs diff=lfs merge=lfs -text
*.dba filter=lfs diff=lfs merge=lfs -text
*.pak filter=lfs diff=lfs merge=lfs -text
*.dds filter=lfs diff=lfs merge=lfs -text
```

### Source Files

Generally all game asset source files should be added to the `.gitattributes` since they are
not text files. Examples include audio files, images, and 3D models.

```text
# Images Sources
*.jpg filter=lfs diff=lfs merge=lfs -text
*.png filter=lfs diff=lfs merge=lfs -text
*.tif filter=lfs diff=lfs merge=lfs -text

# Audio Sources
*.mp3 filter=lfs diff=lfs merge=lfs -text
*.wav filter=lfs diff=lfs merge=lfs -text
*.ogg filter=lfs diff=lfs merge=lfs -text

# Video Sources
*.mp4 filter=lfs diff=lfs merge=lfs -text
*.mov filter=lfs diff=lfs merge=lfs -text

# 3D Object Sources
*.fbx filter=lfs diff=lfs merge=lfs -text
*.obj filter=lfs diff=lfs merge=lfs -text
```
