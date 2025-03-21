# urchin-tool-chain-patches
cd <binutils-dir>

patch -p1 < /patch/to/urchin-toolcahin-patches/binutils/00urchin.patch

cd <gcc-dir>

patch -p1 < /patch/to/urchin-toolcahin-patches/gcc/00urchin.patch


Or if using gentoo with crossdev

mkdir -p /etc/portage/patches/sys-devel/{binutils,gcc}

sudo cp binutils/00urchin.patch /etc/portage/patches/sys-devel/binutils/
sudo cp gcc/00urchin.patch /etc/portage/patches/sys-devel/gcc/
