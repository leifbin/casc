# frozen_string_literal: true

require 'time'

task default: %w[push]

task :push do
  system 'git pull'
  system 'git add .'
  system "git commit -m \"Update #{Time.now}.\""
  system 'git push origin main'
end

task :run do
  system 'git pull'
  # system 'ansible-playbook account.yml'
  system 'ansible-playbook system.yml'
  # system 'ansible-playbook filebeat-new.yml'
  # system 'ansible-playbook fluentd.yml'
  # system 'ansible-playbook video-monitor.yml'
  # system 'ansible-playbook db.yml'
end
