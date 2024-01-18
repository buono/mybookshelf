FROM python:3.8
#FROM debian:10

# コンテナ内にディレクトリを作成
RUN mkdir /work

# コンテナ内の作業ディレクトリを指定
WORKDIR /work

# webディレクトリをコンテナの/workにコピー
ADD web /work


# requirements.txtにリストされたパッケージをインストール
COPY requirements.txt /web/
RUN pip install -r /web/requirements.txt

# add test comment
COPY ***