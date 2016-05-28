#!/usr/bin/env rake
# frozen_string_literal: true
begin
  require 'bundler/setup'
  Bundler.require
rescue LoadError
  puts 'You must `gem install bundler` and `bundle install` to run rake tasks'
end

require 'yard'
YARD::Rake::YardocTask.new(:doc)

require 'rake/testtask'

Rake::TestTask.new do |t|
  t.pattern = 'test/*_test.rb'
end

task default: :test
