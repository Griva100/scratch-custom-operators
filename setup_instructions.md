# Setup Instructions

## 1️⃣ Clone Scratch Repositories
Clone the official Scratch repositories:

```bash
git clone https://github.com/scratchfoundation/scratch-gui.git
git clone https://github.com/scratchfoundation/scratch-vm.git
git clone https://github.com/scratchfoundation/scratch-blocks.git
```

## 2️⃣ Apply Modifications
Copy the modified files into the corresponding directories:

```bash
cp modified-files/scratch-blocks/blocks_vertical/operators.js scratch-blocks/blocks_vertical/
cp modified-files/scratch-vm/src/blocks/scratch3_operators.js scratch-vm/src/blocks/
cp modified-files/scratch-gui/src/lib/libraries/extensions/index.jsx scratch-gui/src/lib/libraries/extensions/
cp modified-files/scratch-gui/src/containers/extension-library.jsx scratch-gui/src/containers/
```
## 3️⃣ Build & Run
Rebuild scratch-blocks

```bash
cd scratch-blocks
npm run prepublish
```

Restart the Project

```bash
cd scratch-gui
npm start
```

## 4️⃣ Create a `.gitignore` File**
```bash
touch .gitignore
```

Add the following content:
```
node_modules/
scratch-gui/node_modules/
scratch-vm/node_modules/
scratch-blocks/node_modules/
scratch-gui/build/
scratch-vm/build/
scratch-blocks/build/
.cache/
*.log
```


