# Changelog

## [0.15.0](https://www.github.com/sentriz/gonic/compare/v0.14.0...v0.15.0) (2022-11-17)


### ⚠ BREAKING CHANGES

* upgrade deps and require go 1.19
* **podcast:** make podcasts global not per user, to match spec

### Features

* add a ping endpoint that doesn't create a session ([731a696](https://www.github.com/sentriz/gonic/commit/731a696bd795bbec668e4685ed1cb2271044c8aa))
* add CreatedAt to albums ([#159](https://www.github.com/sentriz/gonic/issues/159)) ([848d85d](https://www.github.com/sentriz/gonic/commit/848d85d26a4c2a6e83cd01c21e63080fdbb27cd8))
* add multi folder support ([40cd031](https://www.github.com/sentriz/gonic/commit/40cd031b05c71d930b5d92ed6ebbbf676f5e219e)), closes [#50](https://www.github.com/sentriz/gonic/issues/50)
* **countrw:** add countrw package ([5155dee](https://www.github.com/sentriz/gonic/commit/5155dee2e82972ef50adfdbe2298b1126dcd994d))
* **jukebox:** allow users to pass custom arguments to mpv ([428fdda](https://www.github.com/sentriz/gonic/commit/428fddad1bad0dc7091528794622fc2d2dc7c1dc)), closes [#125](https://www.github.com/sentriz/gonic/issues/125) [#164](https://www.github.com/sentriz/gonic/issues/164)
* **jukebox:** use mpv over ipc as a player backend ([e1488b0](https://www.github.com/sentriz/gonic/commit/e1488b0d183a3244eba89220ad960865b94087e5))
* **lastfm:** scrobble with duration ([7d0d036](https://www.github.com/sentriz/gonic/commit/7d0d036f0bc0f5bd4429f510ca636daa3934766b))
* log all folders while scanning ([b2388e6](https://www.github.com/sentriz/gonic/commit/b2388e6d851c2192bda14eb7771c83ce75f493f9))
* **mockfs:** add DumpDB method ([b0d5861](https://www.github.com/sentriz/gonic/commit/b0d5861d10a5472d4ac07a5e27331ec492be69b6))
* **podcasts:** add an option to purge old episodes ([85cb0fe](https://www.github.com/sentriz/gonic/commit/85cb0feb5a11b753bc7936e040e00e95e6601b47))
* render local artist images for getArtistInfo2 ([cb6b33a](https://www.github.com/sentriz/gonic/commit/cb6b33a9fb69589bf73e33773c6f16bf073ce865))
* render local artist images with no foreign key ([a74b5a2](https://www.github.com/sentriz/gonic/commit/a74b5a261c5d47c1a24942ecd4ddd98666755ad4))
* **scanner:** add fuzzing test ([f7f4b8b](https://www.github.com/sentriz/gonic/commit/f7f4b8b2cc3fffaa85a63fceba1bdc7cd79c9044))
* **scanner:** add option to use fsnotify based scan watcher ([#232](https://www.github.com/sentriz/gonic/issues/232)) ([ea28ff1](https://www.github.com/sentriz/gonic/commit/ea28ff1df3f0ea30c53bc79c2e9980ea7ad7206b))
* **scanner:** added option to scan at startup ([f6c9550](https://www.github.com/sentriz/gonic/commit/f6c95503c714dce11bddc4db632028ab09992093)), closes [#251](https://www.github.com/sentriz/gonic/issues/251)
* **server:** support TLS ([59c4047](https://www.github.com/sentriz/gonic/commit/59c404749fa71416e29facac4ec523acd65a0f01))
* **subsonic:** add avatar support ([5e66261](https://www.github.com/sentriz/gonic/commit/5e66261f0ccd63e6ceda46dc908661a748c16325)), closes [#228](https://www.github.com/sentriz/gonic/issues/228)
* **subsonic:** add detailed logging about requested audio ([dc4d9e4](https://www.github.com/sentriz/gonic/commit/dc4d9e4e96c905f6edcfcdddae0a16214b3b054d)), closes [#212](https://www.github.com/sentriz/gonic/issues/212)
* **subsonic:** add getNewestPodcasts ([f6687df](https://www.github.com/sentriz/gonic/commit/f6687df3f3f0d94a2db661b9d4b276175d951d68))
* **subsonic:** add internet radio support ([7ab378a](https://www.github.com/sentriz/gonic/commit/7ab378accbadf2f25478ae37e231aacca881f7b7))
* **subsonic:** add support for track/album/artist ratings/stars ([e8759cb](https://www.github.com/sentriz/gonic/commit/e8759cb6c11cd61a2a8ca3892fc905c4a9c4b167))
* **subsonic:** add year and genre fields to track-by-folder response ([53a4247](https://www.github.com/sentriz/gonic/commit/53a4247dfd18d0783316d6a38126eca3f9df8af9)), closes [#223](https://www.github.com/sentriz/gonic/issues/223)
* **subsonic:** implement getSimilarSongs.view ([e1cfed7](https://www.github.com/sentriz/gonic/commit/e1cfed7965ed43c91689fd5949dab55fa77a983d)), closes [#195](https://www.github.com/sentriz/gonic/issues/195)
* **subsonic:** implement getSimilarSongs2.view ([92febcf](https://www.github.com/sentriz/gonic/commit/92febcffe6bbaff487b6869fbd3467003c987bed)), closes [#195](https://www.github.com/sentriz/gonic/issues/195)
* **subsonic:** implement getTopSongs.view ([39b3ae5](https://www.github.com/sentriz/gonic/commit/39b3ae5ecb2ddb8c733beb99c80b68356d203be2)), closes [#195](https://www.github.com/sentriz/gonic/issues/195)
* **subsonic:** improve getArtistInfo2.view similar artist results ([#203](https://www.github.com/sentriz/gonic/issues/203)) ([55c0920](https://www.github.com/sentriz/gonic/commit/55c09209b6ebdc0ecd7ca17d5b173a8db0cb23b1))
* **subsonic:** log error responses ([2440e69](https://www.github.com/sentriz/gonic/commit/2440e696892b38d2cc255373f700c2449a98fef2))
* **subsonic:** make the v param optional ([50e2818](https://www.github.com/sentriz/gonic/commit/50e2818cc78aad1c5ecdb388dd0ebb5e16f0ae26))
* **subsonic:** return transcoded mime and transcoded suffix in subsonic responses ([6e6404a](https://www.github.com/sentriz/gonic/commit/6e6404af73357b4abcf0d45d2e8114f4404d1b5c))
* **subsonic:** skip transcoding if request bitrate is the same as track bitrate ([f41dd08](https://www.github.com/sentriz/gonic/commit/f41dd0818ba95e27fbad376438585a1057f60382)), closes [#241](https://www.github.com/sentriz/gonic/issues/241)
* **subsonic:** sort artist album list ([e56f64a](https://www.github.com/sentriz/gonic/commit/e56f64a75877efe15f96414c5dc58a33b03cb9ce)), closes [#197](https://www.github.com/sentriz/gonic/issues/197)
* **subsonic:** support dsub edgecase for queries by decade ([03df207](https://www.github.com/sentriz/gonic/commit/03df207e638122446a9b24facfd0b893ddd9e0e8))
* **subsonic:** support public playlists ([1647eaa](https://www.github.com/sentriz/gonic/commit/1647eaac4585cca7a244036f9c242a5602706b83))
* **subsonic:** update play stats when scrobbling ([1ab47d6](https://www.github.com/sentriz/gonic/commit/1ab47d6fbee83f2dd00256bf5cd9ad33c2448202)), closes [#207](https://www.github.com/sentriz/gonic/issues/207)
* **transcode:** add a generic transcoding package for encoding/decoding/caching ([165904c](https://www.github.com/sentriz/gonic/commit/165904c2bb2857aacc9053759ff707d64389a3bb))
* **transcode:** add opus 128 kbps profiles ([bb83426](https://www.github.com/sentriz/gonic/commit/bb83426816a3f5fd45f14a5114e6843923598b21)), closes [#241](https://www.github.com/sentriz/gonic/issues/241)
* **ui:** add a link to wiki in transcode profile section ([3348ca6](https://www.github.com/sentriz/gonic/commit/3348ca6b5bf0d054c8be38e860acdecc6e040b1c)), closes [#254](https://www.github.com/sentriz/gonic/issues/254)
* **ui:** show when a scan is in progress ([7fbe7c0](https://www.github.com/sentriz/gonic/commit/7fbe7c0994356e5adaaa160e51ac4ae051ea027b))
* use album create time for home ui and album listings ([14a2668](https://www.github.com/sentriz/gonic/commit/14a266842600fae27a134590d69542dc5d0d2cfc)), closes [#182](https://www.github.com/sentriz/gonic/issues/182) [#135](https://www.github.com/sentriz/gonic/issues/135)


### Bug Fixes

* add stub getStarred views to shut up refix ([27ac8e1](https://www.github.com/sentriz/gonic/commit/27ac8e1d25d9b58a8c71b9f7318a6b398f4a5865))
* **ci:** set golangci-lint timeout ([48c34fd](https://www.github.com/sentriz/gonic/commit/48c34fdffc1c9bc47ce57d26b433dbbd775831a6))
* **docs:** add GONIC_HTTP_LOG to setting table ([a11d6ab](https://www.github.com/sentriz/gonic/commit/a11d6ab92d3661d2311a1567bf8fffa07dd1eee6))
* don't send listenbrainz playing_now and submitted_at at the same time ([b07b9a8](https://www.github.com/sentriz/gonic/commit/b07b9a8be610a932d6c66839f020456ff136d2f6)), closes [#168](https://www.github.com/sentriz/gonic/issues/168)
* **lastfm:** make a better guess at callback protocol when incoming connection is TLS ([4658d07](https://www.github.com/sentriz/gonic/commit/4658d0727323fdf8107f94c7b0a61c419e6504f6)), closes [#213](https://www.github.com/sentriz/gonic/issues/213)
* **listenbrainz:** set json header ([e883de8](https://www.github.com/sentriz/gonic/commit/e883de8c957a23d14103e547c7ddbbab161a43db))
* **listenbrainz:** submit track recording ID instead of track ID ([8ee357b](https://www.github.com/sentriz/gonic/commit/8ee357b0217eeeebbee954111e17e4d29ac09c91)), closes [#240](https://www.github.com/sentriz/gonic/issues/240)
* make sure open cover and audio files are closed after use ([1d1ab11](https://www.github.com/sentriz/gonic/commit/1d1ab116cd331fb5dbce50051f61be42e771ff80))
* **podcast:** add error case for when DownloadEpisode is called via API and podcast is already downloaded ([611bc96](https://www.github.com/sentriz/gonic/commit/611bc96e29abd69e322b0a33705c164b1577dd99)), closes [#213](https://www.github.com/sentriz/gonic/issues/213)
* **podcast:** add user agent to avoid 403s with some remotes ([0f80ae2](https://www.github.com/sentriz/gonic/commit/0f80ae2655509ddcc044c4e113f5ec1eaed77050))
* render artistId in track types ([7ec6440](https://www.github.com/sentriz/gonic/commit/7ec6440ed2c95b0f38b8089c17dcd23a2d26bf23)), closes [#170](https://www.github.com/sentriz/gonic/issues/170)
* **scanner:** better detect years given extraneous year tags ([a9d3933](https://www.github.com/sentriz/gonic/commit/a9d393350a0286d77d8eb1c68d46e5eb4c2e5cc8))
* **scanner:** fix linting Ctim.Sec/Ctim.Nsec on 32 bit systems ([b280e8d](https://www.github.com/sentriz/gonic/commit/b280e8d256d28cfff6d135d8bf5eadc576e34d45))
* **scanner:** fix records with album name same as artist ([fdbb282](https://www.github.com/sentriz/gonic/commit/fdbb28209b3e155825fa5380774102e2f119e22e)), closes [#230](https://www.github.com/sentriz/gonic/issues/230)
* **scanner:** make sure we have an album artist before populating track ([01747c8](https://www.github.com/sentriz/gonic/commit/01747c89400decedaaa0f801bb9aeb8a7f6e75f5)), closes [#209](https://www.github.com/sentriz/gonic/issues/209)
* **scanner:** respect "is full" setting ([f2143e3](https://www.github.com/sentriz/gonic/commit/f2143e32ef42ae25875db62a2337a4770e095798))
* set ON DELETE SET NULL to artists.guessed_folder_id removing folders ([24d64e2](https://www.github.com/sentriz/gonic/commit/24d64e2125995bbe446fcadc449cc0914a70202c))
* show artist album count when searching by tags ([0c79044](https://www.github.com/sentriz/gonic/commit/0c790442f4fc0c53dd0c71c05b66c600db883b9a))
* show artist covers (raw url in artist info, cover id elsewhere) via scanned guessed artist folder ([c0ebd26](https://www.github.com/sentriz/gonic/commit/c0ebd2642206f7dba81f136cd9d576ded75bb14e)), closes [#180](https://www.github.com/sentriz/gonic/issues/180) [#179](https://www.github.com/sentriz/gonic/issues/179)
* **subsonic:** change order of fromYear toYear query ([d7655cb](https://www.github.com/sentriz/gonic/commit/d7655cb9d167222446c32a21eb4951b75e12857d)), closes [#208](https://www.github.com/sentriz/gonic/issues/208)
* **subsonic:** correct album orderding in getAlbumList, add starred request type in getAlbumList ([692ec68](https://www.github.com/sentriz/gonic/commit/692ec68282805e2dc3cf4a74ac7a44a249fe3695))
* **subsonic:** return an error when no tracks provided in savePlayQueue ([d47d5e1](https://www.github.com/sentriz/gonic/commit/d47d5e17e91d1775e3c6f16d900ba3b565401393))
* **subsonic:** return song artist ID, album and song genres from search3 ([1a1f39f](https://www.github.com/sentriz/gonic/commit/1a1f39f4e8e5553f32499b1461d227a93820e70f)), closes [#229](https://www.github.com/sentriz/gonic/issues/229)
* **subsonic:** route settings.view -> admin home ([f9133aa](https://www.github.com/sentriz/gonic/commit/f9133aac91e5f18473dc461a6f2ffd0417967465))


### Code Refactoring

* **podcast:** make podcasts global not per user, to match spec ([182c96e](https://www.github.com/sentriz/gonic/commit/182c96e9669369d862787f46b541b5090cd64887))


### Miscellaneous Chores

* upgrade deps and require go 1.19 ([385a980](https://www.github.com/sentriz/gonic/commit/385a980b715e7259f896198b4ad4624c40e1e9dd))

## [0.14.0](https://www.github.com/sentriz/gonic/compare/v0.13.1...v0.14.0) (2021-10-03)


### Features

* **ci:** add debug build workflow ([2780dba](https://www.github.com/sentriz/gonic/commit/2780dba534b673b1a496d44c9fcc3007fd0f2e62))
* **ci:** pin golangci-lint version ([8f7131e](https://www.github.com/sentriz/gonic/commit/8f7131e25b9ea4207cdb9091ccbae26b5118cdac))
* **ci:** test before release please, and only run extra tests on develop and pull request ([cd5771f](https://www.github.com/sentriz/gonic/commit/cd5771f88635b95955c7d2aea72379411142b777))
* **ci:** use GITHUB_TOKEN for release please ([608504b](https://www.github.com/sentriz/gonic/commit/608504bedc88ec02cef34849cb42fb476dd63e1c))
* create cache directory on startup ([f3bc3ae](https://www.github.com/sentriz/gonic/commit/f3bc3ae78990948e75d0b9757c399aad4e5c3b6b)), closes [#127](https://www.github.com/sentriz/gonic/issues/127)
* **encode:** add hi-gain RG and upsampling support ([616b152](https://www.github.com/sentriz/gonic/commit/616b152fede7d56b77b8ea96bc2b86226d690f93))
* **encode:** add mime-type headers to cache handlers ([4109b5b](https://www.github.com/sentriz/gonic/commit/4109b5b66cbb53e9255fcd216195f8e1a773e48d))
* **encode:** use "true" (unconstrained) VBR for Opus profiles ([b9f8ea7](https://www.github.com/sentriz/gonic/commit/b9f8ea704876eb033986e7e586f16c93e2864df2))
* **jukebox:** reduce complexity and update dependencies ([#154](https://www.github.com/sentriz/gonic/issues/154)) ([3938136](https://www.github.com/sentriz/gonic/commit/393813665abb614fa2e2f57cdd575c4dd083b4b5))
* support filter by genre in browse by folder mode ([b56f00e](https://www.github.com/sentriz/gonic/commit/b56f00e9ace62fc3d60b21eef7e638b1ec5007d7))
* support filter by year in browse by folder mode ([6e2d4f7](https://www.github.com/sentriz/gonic/commit/6e2d4f73c53ab908b5933cfbbc1ffc97584e0a08))
* Support WMA files, including those with embedded album art ([#143](https://www.github.com/sentriz/gonic/issues/143)) ([7100b2b](https://www.github.com/sentriz/gonic/commit/7100b2b241ab5c199aaa17b2631b85b065b383e1))


### Bug Fixes

* **build:** add zlib ([ccc0e3c](https://www.github.com/sentriz/gonic/commit/ccc0e3c58d9fb1975bc0bdcf4f87829e9f705b74))
* **ci:** remove deprecated linters ([3382af7](https://www.github.com/sentriz/gonic/commit/3382af72f19eead97b601eee847fd60b6c50ca34))
* **ci:** trim short hash ([6f26974](https://www.github.com/sentriz/gonic/commit/6f269745a5f678b256b4a715ba236a2b847e4de9))
* **docs:** update ubuntu / systemd service instructions ([ef6dd6c](https://www.github.com/sentriz/gonic/commit/ef6dd6c82a638dcd8aa3254839e2f53580a4ef46)), closes [#126](https://www.github.com/sentriz/gonic/issues/126)
* **encode:** Strip EBU R128 gain tags when using forced-RG transcoding ([#145](https://www.github.com/sentriz/gonic/issues/145)) ([5444d40](https://www.github.com/sentriz/gonic/commit/5444d40018c6f8051fc8d03ef46bd66737dfe1f4))
* return early before type switch in ServeStream ([212a133](https://www.github.com/sentriz/gonic/commit/212a13395d288486f9baa57c2da9bef2d9b6324d)), closes [#152](https://www.github.com/sentriz/gonic/issues/152)
* **scanner:** refactor a bit and fix the issue of repeatedly adding and removing tracks 😎 ([93608d0](https://www.github.com/sentriz/gonic/commit/93608d04b49ebfde3020752802fd665ccfe807bb)), closes [#26](https://www.github.com/sentriz/gonic/issues/26) [#63](https://www.github.com/sentriz/gonic/issues/63)
* **scanner:** spawn interval scans in a goroutine ([c0ca6aa](https://www.github.com/sentriz/gonic/commit/c0ca6aaf0337a23b3f1d2a867884afe89fd4a281)), closes [#63](https://www.github.com/sentriz/gonic/issues/63)
* **scanner:** update changed cover files when scanning ([f50817a](https://www.github.com/sentriz/gonic/commit/f50817a3dcdaf752ac4c9a20c078428846dc2bde)), closes [#158](https://www.github.com/sentriz/gonic/issues/158)
* show "gonic" not version in --help ([3cf3bda](https://www.github.com/sentriz/gonic/commit/3cf3bdafd890ea25247f2bf9af14e775d8d1d148))
* trim newlines when rendering flag values ([4637cf7](https://www.github.com/sentriz/gonic/commit/4637cf70c16d9c4ea30c9604ca79704ec0e3f0c4))

### [0.13.1](https://www.github.com/sentriz/gonic/compare/v0.13.0...v0.13.1) (2021-05-08)


### Bug Fixes

* **docker:** bump alpine / go ([1f941b2](https://www.github.com/sentriz/gonic/commit/1f941b2085815d8aa0bf7ad7f3e44efba20295e8))

## [0.13.0](https://www.github.com/sentriz/gonic/compare/v0.12.3...v0.13.0) (2021-05-08)


### ⚠ BREAKING CHANGES

* **subsonic:** don't return gonic version from responses
* bump to go1.16 and embed version

### Features

* bump to go1.16 and embed version ([6f15589](https://www.github.com/sentriz/gonic/commit/6f15589c0889893b7beda85a81d49878401566f0))
* **ci:** arm builds, push multiple registries ([0622672](https://www.github.com/sentriz/gonic/commit/06226724b718883cff9e9150e60e2eeacc2e0a1c))
* **ci:** use ghcr and auto release ([c2c7eb2](https://www.github.com/sentriz/gonic/commit/c2c7eb249f77eebabc910c70357249a3017523ef))
* **subsonic:** don't return gonic version from responses ([58624f0](https://www.github.com/sentriz/gonic/commit/58624f07dc81c36fda79827cc41ac57e89e18b37))


### Bug Fixes

* **ci:** only test on go1.16 ([e9743f0](https://www.github.com/sentriz/gonic/commit/e9743f0cb0e96e9b4b434141e890a0fa16ce3f18))
* don't clutter db close in main ([e6b7691](https://www.github.com/sentriz/gonic/commit/e6b76915daa2bbd6f259f2b019cde9130c62e326))
* trim newline from version ([a565008](https://www.github.com/sentriz/gonic/commit/a5650084d7969a37765d291a6554984e4ae4e2d9))
