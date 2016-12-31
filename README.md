# ha

⚠️ WIP - probably not even proof of concept yet

A cli tool to autocomplete host name(s) based on user-defined patterns and freeform(ish) input.

For example, with the pattern `:host.:kind.caius.name`, where `:host` can be anything and `:kind` is `phy` or `vm`, invoking `ha augustus vm` would generate the hostname `augustus.vm.caius.name`. (As would `ha vm augustus`)

## Installation

🤷

## Configuration

* JSON-based configuration
* Placeholder formats can be single strings, arrays of strings or regular expressions
* Define host pattern with placeholders, then define formats/values for placeholders
    * `:node.:app.test`
        * `:node` = `(web|job|cron)\d+`
        * `:app` = `{frontend,api,internal}`
        * Examples

                $ ha web1 api
                web1.api.test
                
                $ ha web{1,2} api cron2
                cron2.api.test
                web1.api.test
                web2.api.test

## Usage

🤷

## License

See LICENSE.
