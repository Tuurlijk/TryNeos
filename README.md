# TryNeos
A Vagrant box to try out the most recent NEOS releases.

Just run `vagrant up` and visit:

* [http://1.2.10.local.neos.io/neos/](http://1.2.10.local.neos.io/neos/)
* [http://2.0.0.local.neos.io/neos/](http://2.0.0.local.neos.io/neos/)

[![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=Tuurlijk&url=https://github.com/Tuurlijk/TryNeos&title=TryNeos&language=Ansible&tags=github&category=software)

## Installation
Installation is pretty straight forward. You're just a couple of steps away from 'great success'.

1). Clone TryNeos and cd into it:
```bash
git clone https://github.com/Tuurlijk/TryNeos.git
cd TryNeos
```

2). Then boot the machine:
```bash
vagrant up
```

3). Now you can visit:

* [http://1.2.10.local.neos.io/neos/](http://1.2.10.local.neos.io/neos/)
* [http://2.0.0.local.neos.io/neos/](http://2.0.0.local.neos.io/neos/)

You can login as user `admin` with the password `supersecret`.

## How do I get onto the box?
You can login by doing a `vagrant ssh`. That user has full sudo privileges. Or you can `ssh vagrant@local.neos.io` using password `vagrant`.

## MailCatcher
[MailCatcher](http://mailcatcher.me/) runs a super simple SMTP server which catches any message sent to it to display in a web interface. This makes it easy to test forms without actually sending mail to the 'real' mail address. Set your favourite app to deliver to smtp://127.0.0.1:1025 instead of your default SMTP server, then check out [http://local.neos.io:1080](http://local.neos.io:1080) to see the mail that's arrived so far.

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests and examples for any new or changed functionality.

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

If you wish to work on the code that built this box, then head over to [https://github.com/Tuurlijk/TYPO3.Packer](https://github.com/Tuurlijk/TYPO3.Packer).
