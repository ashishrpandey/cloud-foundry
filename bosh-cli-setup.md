wget https://github.com/cloudfoundry/bosh-cli/releases/download/v6.1.0/bosh-cli-6.1.0-linux-amd64
mv bosh-cli-6.1.0-linux-amd64 bosh

./bosh -v
chmod +x bosh
mv bosh /usr/local/bin/

bosh -v 
