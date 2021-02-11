FROM ruby:3.0

# Install imap-backup
RUN gem install 'imap-backup' --version 3.2.0

# Make the data directory a volume
VOLUME ["/root/.imap-backup"]

# Add and set the entrypoint
COPY entrypoint.sh /opt/bin/entrypoint.sh
ENTRYPOINT ["/opt/bin/entrypoint.sh"]
