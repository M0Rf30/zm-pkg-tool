Prerequisites:
   sudo apt install dpkg-dev debhelper

Example:
   path../zm-pkg-tool/pkg-build.pl \
      --pkg-version=1.0.2 \
      --pkg-release=1 \
      --pkg-summary="Zimbra Drive Extensions" \
      --pkg-depends='zimbra-core' \
      --pkg-installs='/opt/zimbra/lib/ext/zimbradrive' \
      --pkg-installs='/opt/zimbra/lib/ext/zimbradrive/*' \
      --pkg-installs='/opt/zimbra/zimlets/*'

Test:
   cd e2e-tests && sudo ./TEST.sh
