# Changelog

## [1.1.0](https://github.com/extra2000/misp-box/compare/v1.0.0...v1.1.0) (2021-04-29)


### Features

* **vagrant:** Add Fedora 34 `x86_64` Vagrant file ([a1c5d20](https://github.com/extra2000/misp-box/commit/a1c5d20f60457c4eb438ce9c7f870fcd22a9e9b4))


### Fixes

* **misp-formula:** Patch update to `v1.0.1` ([82c36e2](https://github.com/extra2000/misp-box/commit/82c36e22b027221e9f02a8be307c05be47ffa271))
* **podman-formula:** Patch updates from `v2.2.1` to `v2.2.2` ([a10eb8c](https://github.com/extra2000/misp-box/commit/a10eb8c3bd30031e7355df5f91f233a36f5e0492))


### Continuous Integrations

* **AppVeyor:** Change from Fedora 33 to Fedora 34 ([99e4a33](https://github.com/extra2000/misp-box/commit/99e4a337ff08f86277817920971050e9f72ef4c9))


### Documentations

* **README:** Add instructions how to generate Systemd unit files to auto start Podman pods on boot ([85e5cad](https://github.com/extra2000/misp-box/commit/85e5cada8f8cb849fdc737c9c7abba2d53b63ad9))
* **README:** Move first-time login instructions into Section Initializing MISP ([8be36f2](https://github.com/extra2000/misp-box/commit/8be36f285c11b3e7ffe38a0de801e28d7d0a61db))
* **README:** Set Fedora 34 as default Vagrant instructions ([0320fa2](https://github.com/extra2000/misp-box/commit/0320fa28a75fce9a65a008c87f80e79b0485a373))
* **vagrant:** Add comment for port forwarding ([491bf6c](https://github.com/extra2000/misp-box/commit/491bf6c8ab4fc440289f482beaccbd88b6480eed))

## 1.0.0 (2021-04-19)


### Features

* **salt:** Add implementations for states in `salt/` ([9ca424a](https://github.com/extra2000/misp-box/commit/9ca424a4661c142c477f8b0d3f180c23504d255b))
* **submodule:** Add [misp-formula v1.0.0](https://github.com/extra2000/misp-formula/releases/tag/v1.0.0) ([8e01f08](https://github.com/extra2000/misp-box/commit/8e01f08f80e3f693cd3e32faf85e3a9258b79b1e))
* **submodule:** Add [podman-formula v2.2.1](https://github.com/extra2000/podman-formula/releases/tag/v2.2.1) ([c718713](https://github.com/extra2000/misp-box/commit/c71871378cf71c08f9c5d4bccaacdb8b64fa386a))
* **vagrant:** Import Vagrant files from [extra2000/generic-box v1.7.0](https://github.com/extra2000/generic-box/releases/tag/v1.7.0) ([faf2b1f](https://github.com/extra2000/misp-box/commit/faf2b1f8d5a5d28ed54890ba50c018c1744d97c1))


### Continuous Integrations

* Add AppVeyor with `semantic-release` bot ([0c0112e](https://github.com/extra2000/misp-box/commit/0c0112eeb31001f2d5bff049cf98cd184a876968))


### Documentations

* **README:** Update `README.md` ([1507176](https://github.com/extra2000/misp-box/commit/1507176a2a953f8fac73394edb008bc9ebf7f32b))
