### Scafrando Weblog

# requirements

## actors

- Admin
  ### actions
  - can create post
  - can updte post
  - can eliminate post
  - can fetch posts
  - can comment to a post
  - can delete a post's comments
- Readers

  ### actions

  - can read post
  - can comment post
  - can react a post

## entities

- admin
  ###### properties
  - name => string
  - username => string
  - password => string
  - email => string
- reader
  ###### properties
  - username => string
  - oauth_token => string
- post
  ###### properties
  - link => string
  - tags => string
  - title => string
  - body => string
  - highlights => string
- comment
  ###### properties
  - author => string
  - body => string
  - highlights => string
  - post_id => string
