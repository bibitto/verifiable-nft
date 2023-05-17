1. npm packages をインストール
   $ yarn
2. cert-issuer をインストール
   $ pyenv local 3.9.13
   $ python -m venv venv
   $ source venv/bin/activate
   $ pip install --upgrade pip
   $ env LDFLAGS="-L$(brew --prefix openssl)/lib" CFLAGS="-I$(brew --prefix openssl)/include" pip --no-cache-dir install -r requirements.txt
   $ cert-issuer -h
