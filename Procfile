web: bundle exec unicorn_rails -p ${PORT} -E ${RAILS_ENV} -c ${UNICORN_CONFIG:="config/unicorn.rb"}
worker: bundle exec sidekiq -q post_receive,mailer,system_hook,project_web_hook,common,default,gitlab_shell
