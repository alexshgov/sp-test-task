[![Build Status](https://travis-ci.com/alexshgov/sp-test-task.svg?branch=master)](https://travis-ci.com/alexshgov/sp-test-task)

# Logs parser 

## How to run

```bash
  ruby lib/app.rb --l path_to_your_log
```

## Supported logs formats

For now, the only one format is supported:


```bash
# webserver.log

/about 722.247.931.582
/help_page/1 235.313.352.950
/help_page/1 555.576.836.194
/contact 646.865.545.408
/about 646.865.545.408
/index 200.017.277.774
```

## Testing

notes:
* the task has been implemented using TDD approach and has 100% test coverage

Runs specs with the following command:

```bash
  rspec spec
```

## Ideas

* Large files support: Get rid of `File.read` and analyze file by chunks
* Introduce formatters to support different ways of analysis output, for now a simple Hash is getting printed

### License

Available as open source under the terms of the MIT License.
