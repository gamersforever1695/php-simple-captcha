# PHP Simple Captcha 

A php simple captcha implementation that suite to any type of system built on php.

[![Latest Stable Version](https://img.shields.io/packagist/v/LordDashMe/php-simple-captcha.svg?style=flat-square)](https://packagist.org/packages/LordDashMe/php-simple-captcha) [![Minimum PHP Version](https://img.shields.io/badge/php-%3E%3D%205.6-8892BF.svg?style=flat-square)](https://php.net/) [![Build Status](https://img.shields.io/travis/LordDashMe/php-simple-captcha/master.svg?style=flat-square)](https://travis-ci.org/LordDashMe/php-simple-captcha) [![Coverage Status](https://img.shields.io/coveralls/LordDashMe/php-simple-captcha/master.svg?style=flat-square)](https://coveralls.io/github/LordDashMe/php-simple-captcha?branch=master)

## Requirement(s)

- PHP version from 5.6.* up to latest.

## Install

- It's advice to install the package via Composer. Use the command below to install the package:

```txt
composer require lorddashme/php-simple-captcha
```
![Hello World](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEYAAAAUCAAAAAAVAxSkAAABrUlEQVQ4y+3TPUvDQBgH8OdDOGa+oUMgk2MpdHIIgpSUiqC0OKirgxYX8QVFRQRpBRF8KShqLbgIYkUEteCgFVuqUEVxEIkvJFhae3m8S2KbSkcFBw9yHP88+eXucgH8kQZ/jSm4VDaIy9RKCpKac9NKgU4uEJNwhHhK3qvPBVO8rxRWmFXPF+NSM1KVMbwriAMwhDgVcrxeMZm85GR0PhvGJAAmyozJsbsxgNEir4iEjIK0SYqGd8sOR3rJAGN2BCEkOxhxMhpd8Mk0CXtZacxi1hr20mI/rzgnxayoidevcGuHXTC/q6QuYSMt1jC+gBIiMg12v2vb5NlklChiWnhmFZpwvxDGzuUzV8kOg+N8UUvNBp64vy9q3UN7gDXhwWLY2nMC3zRDibfsY7wjEkY79CdMZhrxSqqzxf4ZRPXwzWJirMicDa5KwiPeARygHXKNMQHEy3rMopDR20XNZGbJzUtrwDC/KshlLDWyqdmhxZzCsdYmf2fWZPoxCEDyfIvdtNQH0PRkH6Q51g8rFO3Qzxh2LbItcDCOpmuOsV7ntNaERe3v/lP/zO8yn4N+yNPrekmPAAAAAElFTkSuQmCC)

![SampleCaptcha](data:image/png;base64,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)

## License

This package is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
