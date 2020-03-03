FROM 30818da4877d

#RUN echo "deb http://archive.ubuntu.com/ubuntu raring main universe" > /etc/apt/sources.list
#RUN sed -i'' 's/archive\.ubuntu\.com/us\.archive\.ubuntu\.com/' /etc/apt/sources.list

#RUN apt-get update


#RUN apt-get install -y  openssh-server git-core openssh-client curl
#RUN apt-get install -y build-essential
#RUN apt-get install -y openssl curl zlib1g zlib1g-dev libssl-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt-dev autoconf libc6-dev ncurses-dev automake libtool bison subversion pkg-config
#RUN apt-get install -y nodejs

# install RVM, Ruby, and Bundler
#RUN \curl -sSL https://rvm.io/mpapis.asc | gpg --import -
#RUN \curl -sSL https://rvm.io/pkuczynski.asc | gpg --import -
#RUN \curl -L https://get.rvm.io | bash -s stable
#RUN /bin/bash -l -c "rvm requirements"
#RUN /bin/bash -l -c "rvm install 2.2.4"
#RUN /bin/bash -l -c "gem install bundler -v 1.10.6"
# Copy application code
#RUN mkdir /myapp
#WORKDIR /myapp
#CPY Gemfile /myapp/Gemfile
#COPY Gemfile.lock /myapp/Gemfile.lock
#RUN /bin/bash -l -c "rvm use 2.2.4"
#RUN /bin/bash -l -c "gem install bundler -v 1.10.6"
#RUN /bin/bash -l -c "bundle install"
COPY . /myapp
EXPOSE 3000
CMD ["rails", "server", "-b", "0.0.0.0"]

