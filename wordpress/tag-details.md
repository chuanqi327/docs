<!-- THIS FILE IS GENERATED VIA '.template-helpers/generate-tag-details.pl' -->

# Tags of `wordpress`

-	[`wordpress:4.5.2-apache`](#wordpress452-apache)
-	[`wordpress:4.5.2`](#wordpress452)
-	[`wordpress:4.5-apache`](#wordpress45-apache)
-	[`wordpress:4.5`](#wordpress45)
-	[`wordpress:4-apache`](#wordpress4-apache)
-	[`wordpress:apache`](#wordpressapache)
-	[`wordpress:4`](#wordpress4)
-	[`wordpress:latest`](#wordpresslatest)
-	[`wordpress:4.5.2-fpm`](#wordpress452-fpm)
-	[`wordpress:4.5-fpm`](#wordpress45-fpm)
-	[`wordpress:4-fpm`](#wordpress4-fpm)
-	[`wordpress:fpm`](#wordpressfpm)

## `wordpress:4.5.2-apache`

```console
$ docker pull library/wordpress@sha256:6173ec31e61338612b4771f607471710459dabacd592877b9c39aa9b5a4c92ef
```

-	Total Virtual Size: 520.7 MB (520660320 bytes)
-	Total v2 Content-Length: 177.1 MB (177107442 bytes)

### Layers (33)

#### `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`

```dockerfile
ADD file:dc2eddd5d35b9d66e4db747f5939b2be7f863dcee64c934b0da690f55a23aee8 in /
```

-	Created: Tue, 03 May 2016 20:57:39 GMT
-	Docker Version: 1.9.1
-	Virtual Size: 125.1 MB (125093399 bytes)
-	v2 Blob: `sha256:8b87079b7a06f9b72e3cca2c984c60e118229c60f0bff855d822f758c112b485`
-	v2 Content-Length: 51.4 MB (51355855 bytes)
-	v2 Last-Modified: Tue, 03 May 2016 20:59:55 GMT

#### `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Tue, 03 May 2016 20:57:42 GMT
-	Parent Layer: `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`

```dockerfile
RUN apt-get update && apt-get install -y \
		autoconf \
		file \
		g++ \
		gcc \
		libc-dev \
		make \
		pkg-config \
		re2c \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:08:29 GMT
-	Parent Layer: `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`
-	Docker Version: 1.9.1
-	Virtual Size: 177.8 MB (177788678 bytes)
-	v2 Blob: `sha256:af1704cb90e1fa3243238682e49412335aba819dc71452142be0a48851ba039a`
-	v2 Content-Length: 69.6 MB (69566346 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:08:02 GMT

#### `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`

```dockerfile
RUN apt-get update && apt-get install -y \
		ca-certificates \
		curl \
		libedit2 \
		libsqlite3-0 \
		libxml2 \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:09:15 GMT
-	Parent Layer: `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`
-	Docker Version: 1.9.1
-	Virtual Size: 16.6 MB (16625930 bytes)
-	v2 Blob: `sha256:6acdef7ebe13fb272b2fb6ac4879f5c815a6e97b34f8f7b46fb3408fddaa03eb`
-	v2 Content-Length: 7.8 MB (7820508 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:26 GMT

#### `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`

```dockerfile
ENV PHP_INI_DIR=/usr/local/etc/php
```

-	Created: Wed, 04 May 2016 03:09:16 GMT
-	Parent Layer: `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`

```dockerfile
RUN mkdir -p $PHP_INI_DIR/conf.d
```

-	Created: Wed, 04 May 2016 03:09:18 GMT
-	Parent Layer: `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:4fc566a7c22ab414ecafcea1db51a7687bfff449c21fcba1ca3ffc8f7431fedc`
-	v2 Content-Length: 180.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:15 GMT

#### `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`

```dockerfile
RUN apt-get update && apt-get install -y apache2-bin apache2.2-common --no-install-recommends && rm -rf /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:19:10 GMT
-	Parent Layer: `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 MB (7144258 bytes)
-	v2 Blob: `sha256:b06a1bacee5136cb74c8d381a9edf716a54b0b7e968561171b16371fe2148e0e`
-	v2 Content-Length: 2.8 MB (2844067 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:11 GMT

#### `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`

```dockerfile
RUN rm -rf /var/www/html && mkdir -p /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html && chown -R www-data:www-data /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html
```

-	Created: Wed, 04 May 2016 03:19:12 GMT
-	Parent Layer: `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:c5fc21fb6c0950653e5db96e21275266c2d6725bd22fc72cc7f74a1334270a39`
-	v2 Content-Length: 321.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:05 GMT

#### `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`

```dockerfile
RUN a2dismod mpm_event && a2enmod mpm_prefork
```

-	Created: Wed, 04 May 2016 03:19:14 GMT
-	Parent Layer: `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`
-	Docker Version: 1.9.1
-	Virtual Size: 68.0 B
-	v2 Blob: `sha256:df319b61c8697392699262bcd17786b49f94b0d55adbccc35ca6ebc980cde386`
-	v2 Content-Length: 431.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:00 GMT

#### `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`

```dockerfile
RUN mv /etc/apache2/apache2.conf /etc/apache2/apache2.conf.dist && rm /etc/apache2/conf-enabled/* /etc/apache2/sites-enabled/*
```

-	Created: Wed, 04 May 2016 03:19:15 GMT
-	Parent Layer: `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 KB (7115 bytes)
-	v2 Blob: `sha256:f958e52674095ca585ddb3e453e794a14722b0a58a7cf46677b81452db55cb9b`
-	v2 Content-Length: 3.4 KB (3364 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:57 GMT

#### `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`

```dockerfile
COPY file:cd759b8d41f4b210d6ab9589edc3741a6aa46739a169e73608046d3df8cbadc7 in /etc/apache2/apache2.conf
```

-	Created: Wed, 04 May 2016 03:19:16 GMT
-	Parent Layer: `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`
-	Docker Version: 1.9.1
-	Virtual Size: 1.5 KB (1520 bytes)
-	v2 Blob: `sha256:b06010f04fa85bbea9ae802425f6e747bc4e48476f7a04daa1b6db8236319a51`
-	v2 Content-Length: 867.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:54 GMT

#### `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`

```dockerfile
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`

```dockerfile
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`

```dockerfile
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`

```dockerfile
ENV PHP_VERSION=5.6.21
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`

```dockerfile
ENV PHP_FILENAME=php-5.6.21.tar.xz
```

-	Created: Wed, 04 May 2016 03:54:09 GMT
-	Parent Layer: `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`

```dockerfile
ENV PHP_SHA256=566ff1a486cb0485ed477a91ea292423f77a58671270ff73b74e67e3ce7084f9
```

-	Created: Wed, 04 May 2016 03:54:10 GMT
-	Parent Layer: `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`

```dockerfile
RUN set -xe \
	&& buildDeps=" \
		$PHP_EXTRA_BUILD_DEPS \
		libcurl4-openssl-dev \
		libedit-dev \
		libsqlite3-dev \
		libssl-dev \
		libxml2-dev \
		xz-utils \
	" \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME/from/this/mirror" -o "$PHP_FILENAME" \
	&& echo "$PHP_SHA256 *$PHP_FILENAME" | sha256sum -c - \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME.asc/from/this/mirror" -o "$PHP_FILENAME.asc" \
	&& export GNUPGHOME="$(mktemp -d)" \
	&& for key in $GPG_KEYS; do \
		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; \
	done \
	&& gpg --batch --verify "$PHP_FILENAME.asc" "$PHP_FILENAME" \
	&& rm -r "$GNUPGHOME" "$PHP_FILENAME.asc" \
	&& mkdir -p /usr/src/php \
	&& tar -xf "$PHP_FILENAME" -C /usr/src/php --strip-components=1 \
	&& rm "$PHP_FILENAME" \
	&& cd /usr/src/php \
	&& ./configure \
		--with-config-file-path="$PHP_INI_DIR" \
		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" \
		$PHP_EXTRA_CONFIGURE_ARGS \
		--disable-cgi \
		--enable-mysqlnd \
		--enable-mbstring \
		--with-curl \
		--with-libedit \
		--with-openssl \
		--with-zlib \
	&& make -j"$(nproc)" \
	&& make install \
	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } \
	&& make clean \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps
```

-	Created: Wed, 04 May 2016 03:58:40 GMT
-	Parent Layer: `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`
-	Docker Version: 1.9.1
-	Virtual Size: 157.3 MB (157283614 bytes)
-	v2 Blob: `sha256:17c1b5f8acff40ea4896f49832dcb3603f88682db67cac65231ea688d2b5f096`
-	v2 Content-Length: 33.5 MB (33456893 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:38 GMT

#### `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`

```dockerfile
COPY multi:82b89724359b10e4fa6ed1d5d2d5ab38544995f1ed9288734f40288633831460 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:46 GMT
-	Parent Layer: `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`
-	Docker Version: 1.9.1
-	Virtual Size: 3.6 KB (3582 bytes)
-	v2 Blob: `sha256:2ed292d591c77a4a469bf3943d6b6b6bae8fd7db68447e2bd82295835fc541f7`
-	v2 Content-Length: 1.5 KB (1547 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:04 GMT

#### `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`

```dockerfile
COPY file:7f47595ed3e349ddf206e03fa4cceb50bbc7e82f815fcd7b924339356c688281 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:47 GMT
-	Parent Layer: `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`
-	Docker Version: 1.9.1
-	Virtual Size: 132.0 B
-	v2 Blob: `sha256:5ea0585ac6f234065af27594fc6ce67264271aec816eaf1f0eb5cdd92de79771`
-	v2 Content-Length: 291.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:01 GMT

#### `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`

```dockerfile
WORKDIR /var/www/html
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`

```dockerfile
EXPOSE 80/tcp
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Wed, 04 May 2016 03:58:49 GMT
-	Parent Layer: `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`

```dockerfile
RUN a2enmod rewrite expires
```

-	Created: Thu, 05 May 2016 05:59:49 GMT
-	Parent Layer: `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`
-	Docker Version: 1.9.1
-	Virtual Size: 60.0 B
-	v2 Blob: `sha256:f53bd09519680e814c527a086ebbdb79224f78b7ec18248570700f57287aac58`
-	v2 Content-Length: 325.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:35:05 GMT

#### `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`

```dockerfile
RUN apt-get update && apt-get install -y libpng12-dev libjpeg-dev && rm -rf /var/lib/apt/lists/* \
	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr \
	&& docker-php-ext-install gd mysqli opcache
```

-	Created: Thu, 05 May 2016 06:01:34 GMT
-	Parent Layer: `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`
-	Docker Version: 1.9.1
-	Virtual Size: 14.8 MB (14798027 bytes)
-	v2 Blob: `sha256:93949259a9c2121cd50bddbc28d3d01fae11cee18b3ff1c2ce1df5e90a11e6c9`
-	v2 Content-Length: 4.4 MB (4442966 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 23:35:02 GMT

#### `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`

```dockerfile
RUN { \
		echo 'opcache.memory_consumption=128'; \
		echo 'opcache.interned_strings_buffer=8'; \
		echo 'opcache.max_accelerated_files=4000'; \
		echo 'opcache.revalidate_freq=60'; \
		echo 'opcache.fast_shutdown=1'; \
		echo 'opcache.enable_cli=1'; \
	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
```

-	Created: Thu, 05 May 2016 06:01:36 GMT
-	Parent Layer: `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`
-	Docker Version: 1.9.1
-	Virtual Size: 172.0 B
-	v2 Blob: `sha256:33ea413bdf772998eccb0a0c97178f5e9b4568f46cfbd445fa47775b77e47928`
-	v2 Content-Length: 330.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:34:56 GMT

#### `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`

```dockerfile
VOLUME [/var/www/html]
```

-	Created: Thu, 05 May 2016 06:01:37 GMT
-	Parent Layer: `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`

```dockerfile
ENV WORDPRESS_VERSION=4.5.2
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`

```dockerfile
ENV WORDPRESS_SHA1=bab94003a5d2285f6ae76407e7b1bbb75382c36e
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`

```dockerfile
RUN curl -o wordpress.tar.gz -SL https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz \
	&& echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c - \
	&& tar -xzf wordpress.tar.gz -C /usr/src/ \
	&& rm wordpress.tar.gz \
	&& chown -R www-data:www-data /usr/src/wordpress
```

-	Created: Tue, 10 May 2016 01:26:05 GMT
-	Parent Layer: `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`
-	Docker Version: 1.9.1
-	Virtual Size: 21.9 MB (21908610 bytes)
-	v2 Blob: `sha256:8d937227258e1c2b37b6f1b004620ddc2a58b96d34ae75dc26c7a159d0f56bfc`
-	v2 Content-Length: 7.6 MB (7610147 bytes)
-	v2 Last-Modified: Tue, 10 May 2016 01:55:22 GMT

#### `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`

```dockerfile
COPY file:e4f27140dddd16cd34ce106cb7587b487bdf49693a3436dc23a89fcb0f933d05 in /entrypoint.sh
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`
-	Docker Version: 1.9.1
-	Virtual Size: 5.2 KB (5155 bytes)
-	v2 Blob: `sha256:f79a39a56bc213acb9b5131bb94562383aecb31e2c72086fafd6aa36a9617201`
-	v2 Content-Length: 2.5 KB (2492 bytes)
-	v2 Last-Modified: Thu, 12 May 2016 20:00:20 GMT

#### `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a913b4803726a52dfbf28eb4ad920a302ec4b09235cbc4de4bdb43fcab8d7abc`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Thu, 12 May 2016 19:21:00 GMT
-	Parent Layer: `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

## `wordpress:4.5.2`

```console
$ docker pull library/wordpress@sha256:d5e31fbc2b48ecc6fc01c96d6942ebb8650ec51a7465ea087a53a256c7a2a30f
```

-	Total Virtual Size: 520.7 MB (520660320 bytes)
-	Total v2 Content-Length: 177.1 MB (177107442 bytes)

### Layers (33)

#### `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`

```dockerfile
ADD file:dc2eddd5d35b9d66e4db747f5939b2be7f863dcee64c934b0da690f55a23aee8 in /
```

-	Created: Tue, 03 May 2016 20:57:39 GMT
-	Docker Version: 1.9.1
-	Virtual Size: 125.1 MB (125093399 bytes)
-	v2 Blob: `sha256:8b87079b7a06f9b72e3cca2c984c60e118229c60f0bff855d822f758c112b485`
-	v2 Content-Length: 51.4 MB (51355855 bytes)
-	v2 Last-Modified: Tue, 03 May 2016 20:59:55 GMT

#### `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Tue, 03 May 2016 20:57:42 GMT
-	Parent Layer: `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`

```dockerfile
RUN apt-get update && apt-get install -y \
		autoconf \
		file \
		g++ \
		gcc \
		libc-dev \
		make \
		pkg-config \
		re2c \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:08:29 GMT
-	Parent Layer: `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`
-	Docker Version: 1.9.1
-	Virtual Size: 177.8 MB (177788678 bytes)
-	v2 Blob: `sha256:af1704cb90e1fa3243238682e49412335aba819dc71452142be0a48851ba039a`
-	v2 Content-Length: 69.6 MB (69566346 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:08:02 GMT

#### `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`

```dockerfile
RUN apt-get update && apt-get install -y \
		ca-certificates \
		curl \
		libedit2 \
		libsqlite3-0 \
		libxml2 \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:09:15 GMT
-	Parent Layer: `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`
-	Docker Version: 1.9.1
-	Virtual Size: 16.6 MB (16625930 bytes)
-	v2 Blob: `sha256:6acdef7ebe13fb272b2fb6ac4879f5c815a6e97b34f8f7b46fb3408fddaa03eb`
-	v2 Content-Length: 7.8 MB (7820508 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:26 GMT

#### `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`

```dockerfile
ENV PHP_INI_DIR=/usr/local/etc/php
```

-	Created: Wed, 04 May 2016 03:09:16 GMT
-	Parent Layer: `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`

```dockerfile
RUN mkdir -p $PHP_INI_DIR/conf.d
```

-	Created: Wed, 04 May 2016 03:09:18 GMT
-	Parent Layer: `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:4fc566a7c22ab414ecafcea1db51a7687bfff449c21fcba1ca3ffc8f7431fedc`
-	v2 Content-Length: 180.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:15 GMT

#### `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`

```dockerfile
RUN apt-get update && apt-get install -y apache2-bin apache2.2-common --no-install-recommends && rm -rf /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:19:10 GMT
-	Parent Layer: `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 MB (7144258 bytes)
-	v2 Blob: `sha256:b06a1bacee5136cb74c8d381a9edf716a54b0b7e968561171b16371fe2148e0e`
-	v2 Content-Length: 2.8 MB (2844067 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:11 GMT

#### `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`

```dockerfile
RUN rm -rf /var/www/html && mkdir -p /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html && chown -R www-data:www-data /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html
```

-	Created: Wed, 04 May 2016 03:19:12 GMT
-	Parent Layer: `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:c5fc21fb6c0950653e5db96e21275266c2d6725bd22fc72cc7f74a1334270a39`
-	v2 Content-Length: 321.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:05 GMT

#### `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`

```dockerfile
RUN a2dismod mpm_event && a2enmod mpm_prefork
```

-	Created: Wed, 04 May 2016 03:19:14 GMT
-	Parent Layer: `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`
-	Docker Version: 1.9.1
-	Virtual Size: 68.0 B
-	v2 Blob: `sha256:df319b61c8697392699262bcd17786b49f94b0d55adbccc35ca6ebc980cde386`
-	v2 Content-Length: 431.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:00 GMT

#### `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`

```dockerfile
RUN mv /etc/apache2/apache2.conf /etc/apache2/apache2.conf.dist && rm /etc/apache2/conf-enabled/* /etc/apache2/sites-enabled/*
```

-	Created: Wed, 04 May 2016 03:19:15 GMT
-	Parent Layer: `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 KB (7115 bytes)
-	v2 Blob: `sha256:f958e52674095ca585ddb3e453e794a14722b0a58a7cf46677b81452db55cb9b`
-	v2 Content-Length: 3.4 KB (3364 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:57 GMT

#### `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`

```dockerfile
COPY file:cd759b8d41f4b210d6ab9589edc3741a6aa46739a169e73608046d3df8cbadc7 in /etc/apache2/apache2.conf
```

-	Created: Wed, 04 May 2016 03:19:16 GMT
-	Parent Layer: `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`
-	Docker Version: 1.9.1
-	Virtual Size: 1.5 KB (1520 bytes)
-	v2 Blob: `sha256:b06010f04fa85bbea9ae802425f6e747bc4e48476f7a04daa1b6db8236319a51`
-	v2 Content-Length: 867.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:54 GMT

#### `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`

```dockerfile
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`

```dockerfile
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`

```dockerfile
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`

```dockerfile
ENV PHP_VERSION=5.6.21
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`

```dockerfile
ENV PHP_FILENAME=php-5.6.21.tar.xz
```

-	Created: Wed, 04 May 2016 03:54:09 GMT
-	Parent Layer: `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`

```dockerfile
ENV PHP_SHA256=566ff1a486cb0485ed477a91ea292423f77a58671270ff73b74e67e3ce7084f9
```

-	Created: Wed, 04 May 2016 03:54:10 GMT
-	Parent Layer: `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`

```dockerfile
RUN set -xe \
	&& buildDeps=" \
		$PHP_EXTRA_BUILD_DEPS \
		libcurl4-openssl-dev \
		libedit-dev \
		libsqlite3-dev \
		libssl-dev \
		libxml2-dev \
		xz-utils \
	" \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME/from/this/mirror" -o "$PHP_FILENAME" \
	&& echo "$PHP_SHA256 *$PHP_FILENAME" | sha256sum -c - \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME.asc/from/this/mirror" -o "$PHP_FILENAME.asc" \
	&& export GNUPGHOME="$(mktemp -d)" \
	&& for key in $GPG_KEYS; do \
		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; \
	done \
	&& gpg --batch --verify "$PHP_FILENAME.asc" "$PHP_FILENAME" \
	&& rm -r "$GNUPGHOME" "$PHP_FILENAME.asc" \
	&& mkdir -p /usr/src/php \
	&& tar -xf "$PHP_FILENAME" -C /usr/src/php --strip-components=1 \
	&& rm "$PHP_FILENAME" \
	&& cd /usr/src/php \
	&& ./configure \
		--with-config-file-path="$PHP_INI_DIR" \
		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" \
		$PHP_EXTRA_CONFIGURE_ARGS \
		--disable-cgi \
		--enable-mysqlnd \
		--enable-mbstring \
		--with-curl \
		--with-libedit \
		--with-openssl \
		--with-zlib \
	&& make -j"$(nproc)" \
	&& make install \
	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } \
	&& make clean \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps
```

-	Created: Wed, 04 May 2016 03:58:40 GMT
-	Parent Layer: `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`
-	Docker Version: 1.9.1
-	Virtual Size: 157.3 MB (157283614 bytes)
-	v2 Blob: `sha256:17c1b5f8acff40ea4896f49832dcb3603f88682db67cac65231ea688d2b5f096`
-	v2 Content-Length: 33.5 MB (33456893 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:38 GMT

#### `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`

```dockerfile
COPY multi:82b89724359b10e4fa6ed1d5d2d5ab38544995f1ed9288734f40288633831460 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:46 GMT
-	Parent Layer: `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`
-	Docker Version: 1.9.1
-	Virtual Size: 3.6 KB (3582 bytes)
-	v2 Blob: `sha256:2ed292d591c77a4a469bf3943d6b6b6bae8fd7db68447e2bd82295835fc541f7`
-	v2 Content-Length: 1.5 KB (1547 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:04 GMT

#### `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`

```dockerfile
COPY file:7f47595ed3e349ddf206e03fa4cceb50bbc7e82f815fcd7b924339356c688281 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:47 GMT
-	Parent Layer: `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`
-	Docker Version: 1.9.1
-	Virtual Size: 132.0 B
-	v2 Blob: `sha256:5ea0585ac6f234065af27594fc6ce67264271aec816eaf1f0eb5cdd92de79771`
-	v2 Content-Length: 291.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:01 GMT

#### `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`

```dockerfile
WORKDIR /var/www/html
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`

```dockerfile
EXPOSE 80/tcp
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Wed, 04 May 2016 03:58:49 GMT
-	Parent Layer: `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`

```dockerfile
RUN a2enmod rewrite expires
```

-	Created: Thu, 05 May 2016 05:59:49 GMT
-	Parent Layer: `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`
-	Docker Version: 1.9.1
-	Virtual Size: 60.0 B
-	v2 Blob: `sha256:f53bd09519680e814c527a086ebbdb79224f78b7ec18248570700f57287aac58`
-	v2 Content-Length: 325.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:35:05 GMT

#### `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`

```dockerfile
RUN apt-get update && apt-get install -y libpng12-dev libjpeg-dev && rm -rf /var/lib/apt/lists/* \
	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr \
	&& docker-php-ext-install gd mysqli opcache
```

-	Created: Thu, 05 May 2016 06:01:34 GMT
-	Parent Layer: `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`
-	Docker Version: 1.9.1
-	Virtual Size: 14.8 MB (14798027 bytes)
-	v2 Blob: `sha256:93949259a9c2121cd50bddbc28d3d01fae11cee18b3ff1c2ce1df5e90a11e6c9`
-	v2 Content-Length: 4.4 MB (4442966 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 23:35:02 GMT

#### `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`

```dockerfile
RUN { \
		echo 'opcache.memory_consumption=128'; \
		echo 'opcache.interned_strings_buffer=8'; \
		echo 'opcache.max_accelerated_files=4000'; \
		echo 'opcache.revalidate_freq=60'; \
		echo 'opcache.fast_shutdown=1'; \
		echo 'opcache.enable_cli=1'; \
	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
```

-	Created: Thu, 05 May 2016 06:01:36 GMT
-	Parent Layer: `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`
-	Docker Version: 1.9.1
-	Virtual Size: 172.0 B
-	v2 Blob: `sha256:33ea413bdf772998eccb0a0c97178f5e9b4568f46cfbd445fa47775b77e47928`
-	v2 Content-Length: 330.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:34:56 GMT

#### `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`

```dockerfile
VOLUME [/var/www/html]
```

-	Created: Thu, 05 May 2016 06:01:37 GMT
-	Parent Layer: `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`

```dockerfile
ENV WORDPRESS_VERSION=4.5.2
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`

```dockerfile
ENV WORDPRESS_SHA1=bab94003a5d2285f6ae76407e7b1bbb75382c36e
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`

```dockerfile
RUN curl -o wordpress.tar.gz -SL https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz \
	&& echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c - \
	&& tar -xzf wordpress.tar.gz -C /usr/src/ \
	&& rm wordpress.tar.gz \
	&& chown -R www-data:www-data /usr/src/wordpress
```

-	Created: Tue, 10 May 2016 01:26:05 GMT
-	Parent Layer: `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`
-	Docker Version: 1.9.1
-	Virtual Size: 21.9 MB (21908610 bytes)
-	v2 Blob: `sha256:8d937227258e1c2b37b6f1b004620ddc2a58b96d34ae75dc26c7a159d0f56bfc`
-	v2 Content-Length: 7.6 MB (7610147 bytes)
-	v2 Last-Modified: Tue, 10 May 2016 01:55:22 GMT

#### `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`

```dockerfile
COPY file:e4f27140dddd16cd34ce106cb7587b487bdf49693a3436dc23a89fcb0f933d05 in /entrypoint.sh
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`
-	Docker Version: 1.9.1
-	Virtual Size: 5.2 KB (5155 bytes)
-	v2 Blob: `sha256:f79a39a56bc213acb9b5131bb94562383aecb31e2c72086fafd6aa36a9617201`
-	v2 Content-Length: 2.5 KB (2492 bytes)
-	v2 Last-Modified: Thu, 12 May 2016 20:00:20 GMT

#### `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a913b4803726a52dfbf28eb4ad920a302ec4b09235cbc4de4bdb43fcab8d7abc`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Thu, 12 May 2016 19:21:00 GMT
-	Parent Layer: `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

## `wordpress:4.5-apache`

```console
$ docker pull library/wordpress@sha256:e3598980a27abb93ee9ceb5a34fc77e6f39edaa587a2e4cb14285c01ef54982d
```

-	Total Virtual Size: 520.7 MB (520660320 bytes)
-	Total v2 Content-Length: 177.1 MB (177107442 bytes)

### Layers (33)

#### `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`

```dockerfile
ADD file:dc2eddd5d35b9d66e4db747f5939b2be7f863dcee64c934b0da690f55a23aee8 in /
```

-	Created: Tue, 03 May 2016 20:57:39 GMT
-	Docker Version: 1.9.1
-	Virtual Size: 125.1 MB (125093399 bytes)
-	v2 Blob: `sha256:8b87079b7a06f9b72e3cca2c984c60e118229c60f0bff855d822f758c112b485`
-	v2 Content-Length: 51.4 MB (51355855 bytes)
-	v2 Last-Modified: Tue, 03 May 2016 20:59:55 GMT

#### `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Tue, 03 May 2016 20:57:42 GMT
-	Parent Layer: `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`

```dockerfile
RUN apt-get update && apt-get install -y \
		autoconf \
		file \
		g++ \
		gcc \
		libc-dev \
		make \
		pkg-config \
		re2c \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:08:29 GMT
-	Parent Layer: `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`
-	Docker Version: 1.9.1
-	Virtual Size: 177.8 MB (177788678 bytes)
-	v2 Blob: `sha256:af1704cb90e1fa3243238682e49412335aba819dc71452142be0a48851ba039a`
-	v2 Content-Length: 69.6 MB (69566346 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:08:02 GMT

#### `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`

```dockerfile
RUN apt-get update && apt-get install -y \
		ca-certificates \
		curl \
		libedit2 \
		libsqlite3-0 \
		libxml2 \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:09:15 GMT
-	Parent Layer: `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`
-	Docker Version: 1.9.1
-	Virtual Size: 16.6 MB (16625930 bytes)
-	v2 Blob: `sha256:6acdef7ebe13fb272b2fb6ac4879f5c815a6e97b34f8f7b46fb3408fddaa03eb`
-	v2 Content-Length: 7.8 MB (7820508 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:26 GMT

#### `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`

```dockerfile
ENV PHP_INI_DIR=/usr/local/etc/php
```

-	Created: Wed, 04 May 2016 03:09:16 GMT
-	Parent Layer: `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`

```dockerfile
RUN mkdir -p $PHP_INI_DIR/conf.d
```

-	Created: Wed, 04 May 2016 03:09:18 GMT
-	Parent Layer: `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:4fc566a7c22ab414ecafcea1db51a7687bfff449c21fcba1ca3ffc8f7431fedc`
-	v2 Content-Length: 180.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:15 GMT

#### `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`

```dockerfile
RUN apt-get update && apt-get install -y apache2-bin apache2.2-common --no-install-recommends && rm -rf /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:19:10 GMT
-	Parent Layer: `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 MB (7144258 bytes)
-	v2 Blob: `sha256:b06a1bacee5136cb74c8d381a9edf716a54b0b7e968561171b16371fe2148e0e`
-	v2 Content-Length: 2.8 MB (2844067 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:11 GMT

#### `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`

```dockerfile
RUN rm -rf /var/www/html && mkdir -p /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html && chown -R www-data:www-data /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html
```

-	Created: Wed, 04 May 2016 03:19:12 GMT
-	Parent Layer: `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:c5fc21fb6c0950653e5db96e21275266c2d6725bd22fc72cc7f74a1334270a39`
-	v2 Content-Length: 321.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:05 GMT

#### `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`

```dockerfile
RUN a2dismod mpm_event && a2enmod mpm_prefork
```

-	Created: Wed, 04 May 2016 03:19:14 GMT
-	Parent Layer: `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`
-	Docker Version: 1.9.1
-	Virtual Size: 68.0 B
-	v2 Blob: `sha256:df319b61c8697392699262bcd17786b49f94b0d55adbccc35ca6ebc980cde386`
-	v2 Content-Length: 431.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:00 GMT

#### `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`

```dockerfile
RUN mv /etc/apache2/apache2.conf /etc/apache2/apache2.conf.dist && rm /etc/apache2/conf-enabled/* /etc/apache2/sites-enabled/*
```

-	Created: Wed, 04 May 2016 03:19:15 GMT
-	Parent Layer: `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 KB (7115 bytes)
-	v2 Blob: `sha256:f958e52674095ca585ddb3e453e794a14722b0a58a7cf46677b81452db55cb9b`
-	v2 Content-Length: 3.4 KB (3364 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:57 GMT

#### `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`

```dockerfile
COPY file:cd759b8d41f4b210d6ab9589edc3741a6aa46739a169e73608046d3df8cbadc7 in /etc/apache2/apache2.conf
```

-	Created: Wed, 04 May 2016 03:19:16 GMT
-	Parent Layer: `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`
-	Docker Version: 1.9.1
-	Virtual Size: 1.5 KB (1520 bytes)
-	v2 Blob: `sha256:b06010f04fa85bbea9ae802425f6e747bc4e48476f7a04daa1b6db8236319a51`
-	v2 Content-Length: 867.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:54 GMT

#### `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`

```dockerfile
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`

```dockerfile
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`

```dockerfile
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`

```dockerfile
ENV PHP_VERSION=5.6.21
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`

```dockerfile
ENV PHP_FILENAME=php-5.6.21.tar.xz
```

-	Created: Wed, 04 May 2016 03:54:09 GMT
-	Parent Layer: `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`

```dockerfile
ENV PHP_SHA256=566ff1a486cb0485ed477a91ea292423f77a58671270ff73b74e67e3ce7084f9
```

-	Created: Wed, 04 May 2016 03:54:10 GMT
-	Parent Layer: `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`

```dockerfile
RUN set -xe \
	&& buildDeps=" \
		$PHP_EXTRA_BUILD_DEPS \
		libcurl4-openssl-dev \
		libedit-dev \
		libsqlite3-dev \
		libssl-dev \
		libxml2-dev \
		xz-utils \
	" \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME/from/this/mirror" -o "$PHP_FILENAME" \
	&& echo "$PHP_SHA256 *$PHP_FILENAME" | sha256sum -c - \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME.asc/from/this/mirror" -o "$PHP_FILENAME.asc" \
	&& export GNUPGHOME="$(mktemp -d)" \
	&& for key in $GPG_KEYS; do \
		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; \
	done \
	&& gpg --batch --verify "$PHP_FILENAME.asc" "$PHP_FILENAME" \
	&& rm -r "$GNUPGHOME" "$PHP_FILENAME.asc" \
	&& mkdir -p /usr/src/php \
	&& tar -xf "$PHP_FILENAME" -C /usr/src/php --strip-components=1 \
	&& rm "$PHP_FILENAME" \
	&& cd /usr/src/php \
	&& ./configure \
		--with-config-file-path="$PHP_INI_DIR" \
		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" \
		$PHP_EXTRA_CONFIGURE_ARGS \
		--disable-cgi \
		--enable-mysqlnd \
		--enable-mbstring \
		--with-curl \
		--with-libedit \
		--with-openssl \
		--with-zlib \
	&& make -j"$(nproc)" \
	&& make install \
	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } \
	&& make clean \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps
```

-	Created: Wed, 04 May 2016 03:58:40 GMT
-	Parent Layer: `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`
-	Docker Version: 1.9.1
-	Virtual Size: 157.3 MB (157283614 bytes)
-	v2 Blob: `sha256:17c1b5f8acff40ea4896f49832dcb3603f88682db67cac65231ea688d2b5f096`
-	v2 Content-Length: 33.5 MB (33456893 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:38 GMT

#### `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`

```dockerfile
COPY multi:82b89724359b10e4fa6ed1d5d2d5ab38544995f1ed9288734f40288633831460 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:46 GMT
-	Parent Layer: `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`
-	Docker Version: 1.9.1
-	Virtual Size: 3.6 KB (3582 bytes)
-	v2 Blob: `sha256:2ed292d591c77a4a469bf3943d6b6b6bae8fd7db68447e2bd82295835fc541f7`
-	v2 Content-Length: 1.5 KB (1547 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:04 GMT

#### `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`

```dockerfile
COPY file:7f47595ed3e349ddf206e03fa4cceb50bbc7e82f815fcd7b924339356c688281 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:47 GMT
-	Parent Layer: `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`
-	Docker Version: 1.9.1
-	Virtual Size: 132.0 B
-	v2 Blob: `sha256:5ea0585ac6f234065af27594fc6ce67264271aec816eaf1f0eb5cdd92de79771`
-	v2 Content-Length: 291.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:01 GMT

#### `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`

```dockerfile
WORKDIR /var/www/html
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`

```dockerfile
EXPOSE 80/tcp
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Wed, 04 May 2016 03:58:49 GMT
-	Parent Layer: `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`

```dockerfile
RUN a2enmod rewrite expires
```

-	Created: Thu, 05 May 2016 05:59:49 GMT
-	Parent Layer: `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`
-	Docker Version: 1.9.1
-	Virtual Size: 60.0 B
-	v2 Blob: `sha256:f53bd09519680e814c527a086ebbdb79224f78b7ec18248570700f57287aac58`
-	v2 Content-Length: 325.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:35:05 GMT

#### `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`

```dockerfile
RUN apt-get update && apt-get install -y libpng12-dev libjpeg-dev && rm -rf /var/lib/apt/lists/* \
	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr \
	&& docker-php-ext-install gd mysqli opcache
```

-	Created: Thu, 05 May 2016 06:01:34 GMT
-	Parent Layer: `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`
-	Docker Version: 1.9.1
-	Virtual Size: 14.8 MB (14798027 bytes)
-	v2 Blob: `sha256:93949259a9c2121cd50bddbc28d3d01fae11cee18b3ff1c2ce1df5e90a11e6c9`
-	v2 Content-Length: 4.4 MB (4442966 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 23:35:02 GMT

#### `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`

```dockerfile
RUN { \
		echo 'opcache.memory_consumption=128'; \
		echo 'opcache.interned_strings_buffer=8'; \
		echo 'opcache.max_accelerated_files=4000'; \
		echo 'opcache.revalidate_freq=60'; \
		echo 'opcache.fast_shutdown=1'; \
		echo 'opcache.enable_cli=1'; \
	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
```

-	Created: Thu, 05 May 2016 06:01:36 GMT
-	Parent Layer: `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`
-	Docker Version: 1.9.1
-	Virtual Size: 172.0 B
-	v2 Blob: `sha256:33ea413bdf772998eccb0a0c97178f5e9b4568f46cfbd445fa47775b77e47928`
-	v2 Content-Length: 330.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:34:56 GMT

#### `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`

```dockerfile
VOLUME [/var/www/html]
```

-	Created: Thu, 05 May 2016 06:01:37 GMT
-	Parent Layer: `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`

```dockerfile
ENV WORDPRESS_VERSION=4.5.2
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`

```dockerfile
ENV WORDPRESS_SHA1=bab94003a5d2285f6ae76407e7b1bbb75382c36e
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`

```dockerfile
RUN curl -o wordpress.tar.gz -SL https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz \
	&& echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c - \
	&& tar -xzf wordpress.tar.gz -C /usr/src/ \
	&& rm wordpress.tar.gz \
	&& chown -R www-data:www-data /usr/src/wordpress
```

-	Created: Tue, 10 May 2016 01:26:05 GMT
-	Parent Layer: `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`
-	Docker Version: 1.9.1
-	Virtual Size: 21.9 MB (21908610 bytes)
-	v2 Blob: `sha256:8d937227258e1c2b37b6f1b004620ddc2a58b96d34ae75dc26c7a159d0f56bfc`
-	v2 Content-Length: 7.6 MB (7610147 bytes)
-	v2 Last-Modified: Tue, 10 May 2016 01:55:22 GMT

#### `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`

```dockerfile
COPY file:e4f27140dddd16cd34ce106cb7587b487bdf49693a3436dc23a89fcb0f933d05 in /entrypoint.sh
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`
-	Docker Version: 1.9.1
-	Virtual Size: 5.2 KB (5155 bytes)
-	v2 Blob: `sha256:f79a39a56bc213acb9b5131bb94562383aecb31e2c72086fafd6aa36a9617201`
-	v2 Content-Length: 2.5 KB (2492 bytes)
-	v2 Last-Modified: Thu, 12 May 2016 20:00:20 GMT

#### `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a913b4803726a52dfbf28eb4ad920a302ec4b09235cbc4de4bdb43fcab8d7abc`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Thu, 12 May 2016 19:21:00 GMT
-	Parent Layer: `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

## `wordpress:4.5`

```console
$ docker pull library/wordpress@sha256:83c7fd5c29dd668781aebb4b3d48705a95cc3a39818a5ad81ceb4672b384713e
```

-	Total Virtual Size: 520.7 MB (520660320 bytes)
-	Total v2 Content-Length: 177.1 MB (177107442 bytes)

### Layers (33)

#### `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`

```dockerfile
ADD file:dc2eddd5d35b9d66e4db747f5939b2be7f863dcee64c934b0da690f55a23aee8 in /
```

-	Created: Tue, 03 May 2016 20:57:39 GMT
-	Docker Version: 1.9.1
-	Virtual Size: 125.1 MB (125093399 bytes)
-	v2 Blob: `sha256:8b87079b7a06f9b72e3cca2c984c60e118229c60f0bff855d822f758c112b485`
-	v2 Content-Length: 51.4 MB (51355855 bytes)
-	v2 Last-Modified: Tue, 03 May 2016 20:59:55 GMT

#### `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Tue, 03 May 2016 20:57:42 GMT
-	Parent Layer: `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`

```dockerfile
RUN apt-get update && apt-get install -y \
		autoconf \
		file \
		g++ \
		gcc \
		libc-dev \
		make \
		pkg-config \
		re2c \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:08:29 GMT
-	Parent Layer: `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`
-	Docker Version: 1.9.1
-	Virtual Size: 177.8 MB (177788678 bytes)
-	v2 Blob: `sha256:af1704cb90e1fa3243238682e49412335aba819dc71452142be0a48851ba039a`
-	v2 Content-Length: 69.6 MB (69566346 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:08:02 GMT

#### `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`

```dockerfile
RUN apt-get update && apt-get install -y \
		ca-certificates \
		curl \
		libedit2 \
		libsqlite3-0 \
		libxml2 \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:09:15 GMT
-	Parent Layer: `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`
-	Docker Version: 1.9.1
-	Virtual Size: 16.6 MB (16625930 bytes)
-	v2 Blob: `sha256:6acdef7ebe13fb272b2fb6ac4879f5c815a6e97b34f8f7b46fb3408fddaa03eb`
-	v2 Content-Length: 7.8 MB (7820508 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:26 GMT

#### `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`

```dockerfile
ENV PHP_INI_DIR=/usr/local/etc/php
```

-	Created: Wed, 04 May 2016 03:09:16 GMT
-	Parent Layer: `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`

```dockerfile
RUN mkdir -p $PHP_INI_DIR/conf.d
```

-	Created: Wed, 04 May 2016 03:09:18 GMT
-	Parent Layer: `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:4fc566a7c22ab414ecafcea1db51a7687bfff449c21fcba1ca3ffc8f7431fedc`
-	v2 Content-Length: 180.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:15 GMT

#### `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`

```dockerfile
RUN apt-get update && apt-get install -y apache2-bin apache2.2-common --no-install-recommends && rm -rf /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:19:10 GMT
-	Parent Layer: `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 MB (7144258 bytes)
-	v2 Blob: `sha256:b06a1bacee5136cb74c8d381a9edf716a54b0b7e968561171b16371fe2148e0e`
-	v2 Content-Length: 2.8 MB (2844067 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:11 GMT

#### `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`

```dockerfile
RUN rm -rf /var/www/html && mkdir -p /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html && chown -R www-data:www-data /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html
```

-	Created: Wed, 04 May 2016 03:19:12 GMT
-	Parent Layer: `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:c5fc21fb6c0950653e5db96e21275266c2d6725bd22fc72cc7f74a1334270a39`
-	v2 Content-Length: 321.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:05 GMT

#### `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`

```dockerfile
RUN a2dismod mpm_event && a2enmod mpm_prefork
```

-	Created: Wed, 04 May 2016 03:19:14 GMT
-	Parent Layer: `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`
-	Docker Version: 1.9.1
-	Virtual Size: 68.0 B
-	v2 Blob: `sha256:df319b61c8697392699262bcd17786b49f94b0d55adbccc35ca6ebc980cde386`
-	v2 Content-Length: 431.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:00 GMT

#### `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`

```dockerfile
RUN mv /etc/apache2/apache2.conf /etc/apache2/apache2.conf.dist && rm /etc/apache2/conf-enabled/* /etc/apache2/sites-enabled/*
```

-	Created: Wed, 04 May 2016 03:19:15 GMT
-	Parent Layer: `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 KB (7115 bytes)
-	v2 Blob: `sha256:f958e52674095ca585ddb3e453e794a14722b0a58a7cf46677b81452db55cb9b`
-	v2 Content-Length: 3.4 KB (3364 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:57 GMT

#### `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`

```dockerfile
COPY file:cd759b8d41f4b210d6ab9589edc3741a6aa46739a169e73608046d3df8cbadc7 in /etc/apache2/apache2.conf
```

-	Created: Wed, 04 May 2016 03:19:16 GMT
-	Parent Layer: `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`
-	Docker Version: 1.9.1
-	Virtual Size: 1.5 KB (1520 bytes)
-	v2 Blob: `sha256:b06010f04fa85bbea9ae802425f6e747bc4e48476f7a04daa1b6db8236319a51`
-	v2 Content-Length: 867.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:54 GMT

#### `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`

```dockerfile
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`

```dockerfile
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`

```dockerfile
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`

```dockerfile
ENV PHP_VERSION=5.6.21
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`

```dockerfile
ENV PHP_FILENAME=php-5.6.21.tar.xz
```

-	Created: Wed, 04 May 2016 03:54:09 GMT
-	Parent Layer: `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`

```dockerfile
ENV PHP_SHA256=566ff1a486cb0485ed477a91ea292423f77a58671270ff73b74e67e3ce7084f9
```

-	Created: Wed, 04 May 2016 03:54:10 GMT
-	Parent Layer: `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`

```dockerfile
RUN set -xe \
	&& buildDeps=" \
		$PHP_EXTRA_BUILD_DEPS \
		libcurl4-openssl-dev \
		libedit-dev \
		libsqlite3-dev \
		libssl-dev \
		libxml2-dev \
		xz-utils \
	" \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME/from/this/mirror" -o "$PHP_FILENAME" \
	&& echo "$PHP_SHA256 *$PHP_FILENAME" | sha256sum -c - \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME.asc/from/this/mirror" -o "$PHP_FILENAME.asc" \
	&& export GNUPGHOME="$(mktemp -d)" \
	&& for key in $GPG_KEYS; do \
		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; \
	done \
	&& gpg --batch --verify "$PHP_FILENAME.asc" "$PHP_FILENAME" \
	&& rm -r "$GNUPGHOME" "$PHP_FILENAME.asc" \
	&& mkdir -p /usr/src/php \
	&& tar -xf "$PHP_FILENAME" -C /usr/src/php --strip-components=1 \
	&& rm "$PHP_FILENAME" \
	&& cd /usr/src/php \
	&& ./configure \
		--with-config-file-path="$PHP_INI_DIR" \
		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" \
		$PHP_EXTRA_CONFIGURE_ARGS \
		--disable-cgi \
		--enable-mysqlnd \
		--enable-mbstring \
		--with-curl \
		--with-libedit \
		--with-openssl \
		--with-zlib \
	&& make -j"$(nproc)" \
	&& make install \
	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } \
	&& make clean \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps
```

-	Created: Wed, 04 May 2016 03:58:40 GMT
-	Parent Layer: `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`
-	Docker Version: 1.9.1
-	Virtual Size: 157.3 MB (157283614 bytes)
-	v2 Blob: `sha256:17c1b5f8acff40ea4896f49832dcb3603f88682db67cac65231ea688d2b5f096`
-	v2 Content-Length: 33.5 MB (33456893 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:38 GMT

#### `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`

```dockerfile
COPY multi:82b89724359b10e4fa6ed1d5d2d5ab38544995f1ed9288734f40288633831460 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:46 GMT
-	Parent Layer: `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`
-	Docker Version: 1.9.1
-	Virtual Size: 3.6 KB (3582 bytes)
-	v2 Blob: `sha256:2ed292d591c77a4a469bf3943d6b6b6bae8fd7db68447e2bd82295835fc541f7`
-	v2 Content-Length: 1.5 KB (1547 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:04 GMT

#### `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`

```dockerfile
COPY file:7f47595ed3e349ddf206e03fa4cceb50bbc7e82f815fcd7b924339356c688281 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:47 GMT
-	Parent Layer: `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`
-	Docker Version: 1.9.1
-	Virtual Size: 132.0 B
-	v2 Blob: `sha256:5ea0585ac6f234065af27594fc6ce67264271aec816eaf1f0eb5cdd92de79771`
-	v2 Content-Length: 291.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:01 GMT

#### `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`

```dockerfile
WORKDIR /var/www/html
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`

```dockerfile
EXPOSE 80/tcp
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Wed, 04 May 2016 03:58:49 GMT
-	Parent Layer: `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`

```dockerfile
RUN a2enmod rewrite expires
```

-	Created: Thu, 05 May 2016 05:59:49 GMT
-	Parent Layer: `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`
-	Docker Version: 1.9.1
-	Virtual Size: 60.0 B
-	v2 Blob: `sha256:f53bd09519680e814c527a086ebbdb79224f78b7ec18248570700f57287aac58`
-	v2 Content-Length: 325.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:35:05 GMT

#### `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`

```dockerfile
RUN apt-get update && apt-get install -y libpng12-dev libjpeg-dev && rm -rf /var/lib/apt/lists/* \
	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr \
	&& docker-php-ext-install gd mysqli opcache
```

-	Created: Thu, 05 May 2016 06:01:34 GMT
-	Parent Layer: `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`
-	Docker Version: 1.9.1
-	Virtual Size: 14.8 MB (14798027 bytes)
-	v2 Blob: `sha256:93949259a9c2121cd50bddbc28d3d01fae11cee18b3ff1c2ce1df5e90a11e6c9`
-	v2 Content-Length: 4.4 MB (4442966 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 23:35:02 GMT

#### `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`

```dockerfile
RUN { \
		echo 'opcache.memory_consumption=128'; \
		echo 'opcache.interned_strings_buffer=8'; \
		echo 'opcache.max_accelerated_files=4000'; \
		echo 'opcache.revalidate_freq=60'; \
		echo 'opcache.fast_shutdown=1'; \
		echo 'opcache.enable_cli=1'; \
	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
```

-	Created: Thu, 05 May 2016 06:01:36 GMT
-	Parent Layer: `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`
-	Docker Version: 1.9.1
-	Virtual Size: 172.0 B
-	v2 Blob: `sha256:33ea413bdf772998eccb0a0c97178f5e9b4568f46cfbd445fa47775b77e47928`
-	v2 Content-Length: 330.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:34:56 GMT

#### `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`

```dockerfile
VOLUME [/var/www/html]
```

-	Created: Thu, 05 May 2016 06:01:37 GMT
-	Parent Layer: `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`

```dockerfile
ENV WORDPRESS_VERSION=4.5.2
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`

```dockerfile
ENV WORDPRESS_SHA1=bab94003a5d2285f6ae76407e7b1bbb75382c36e
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`

```dockerfile
RUN curl -o wordpress.tar.gz -SL https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz \
	&& echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c - \
	&& tar -xzf wordpress.tar.gz -C /usr/src/ \
	&& rm wordpress.tar.gz \
	&& chown -R www-data:www-data /usr/src/wordpress
```

-	Created: Tue, 10 May 2016 01:26:05 GMT
-	Parent Layer: `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`
-	Docker Version: 1.9.1
-	Virtual Size: 21.9 MB (21908610 bytes)
-	v2 Blob: `sha256:8d937227258e1c2b37b6f1b004620ddc2a58b96d34ae75dc26c7a159d0f56bfc`
-	v2 Content-Length: 7.6 MB (7610147 bytes)
-	v2 Last-Modified: Tue, 10 May 2016 01:55:22 GMT

#### `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`

```dockerfile
COPY file:e4f27140dddd16cd34ce106cb7587b487bdf49693a3436dc23a89fcb0f933d05 in /entrypoint.sh
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`
-	Docker Version: 1.9.1
-	Virtual Size: 5.2 KB (5155 bytes)
-	v2 Blob: `sha256:f79a39a56bc213acb9b5131bb94562383aecb31e2c72086fafd6aa36a9617201`
-	v2 Content-Length: 2.5 KB (2492 bytes)
-	v2 Last-Modified: Thu, 12 May 2016 20:00:20 GMT

#### `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a913b4803726a52dfbf28eb4ad920a302ec4b09235cbc4de4bdb43fcab8d7abc`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Thu, 12 May 2016 19:21:00 GMT
-	Parent Layer: `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

## `wordpress:4-apache`

```console
$ docker pull library/wordpress@sha256:ecd1f7aa850d32c2f0d76194e6acebb73f569609c9d1ce7bf0d0e53e5b6c80d2
```

-	Total Virtual Size: 520.7 MB (520660320 bytes)
-	Total v2 Content-Length: 177.1 MB (177107442 bytes)

### Layers (33)

#### `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`

```dockerfile
ADD file:dc2eddd5d35b9d66e4db747f5939b2be7f863dcee64c934b0da690f55a23aee8 in /
```

-	Created: Tue, 03 May 2016 20:57:39 GMT
-	Docker Version: 1.9.1
-	Virtual Size: 125.1 MB (125093399 bytes)
-	v2 Blob: `sha256:8b87079b7a06f9b72e3cca2c984c60e118229c60f0bff855d822f758c112b485`
-	v2 Content-Length: 51.4 MB (51355855 bytes)
-	v2 Last-Modified: Tue, 03 May 2016 20:59:55 GMT

#### `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Tue, 03 May 2016 20:57:42 GMT
-	Parent Layer: `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`

```dockerfile
RUN apt-get update && apt-get install -y \
		autoconf \
		file \
		g++ \
		gcc \
		libc-dev \
		make \
		pkg-config \
		re2c \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:08:29 GMT
-	Parent Layer: `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`
-	Docker Version: 1.9.1
-	Virtual Size: 177.8 MB (177788678 bytes)
-	v2 Blob: `sha256:af1704cb90e1fa3243238682e49412335aba819dc71452142be0a48851ba039a`
-	v2 Content-Length: 69.6 MB (69566346 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:08:02 GMT

#### `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`

```dockerfile
RUN apt-get update && apt-get install -y \
		ca-certificates \
		curl \
		libedit2 \
		libsqlite3-0 \
		libxml2 \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:09:15 GMT
-	Parent Layer: `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`
-	Docker Version: 1.9.1
-	Virtual Size: 16.6 MB (16625930 bytes)
-	v2 Blob: `sha256:6acdef7ebe13fb272b2fb6ac4879f5c815a6e97b34f8f7b46fb3408fddaa03eb`
-	v2 Content-Length: 7.8 MB (7820508 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:26 GMT

#### `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`

```dockerfile
ENV PHP_INI_DIR=/usr/local/etc/php
```

-	Created: Wed, 04 May 2016 03:09:16 GMT
-	Parent Layer: `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`

```dockerfile
RUN mkdir -p $PHP_INI_DIR/conf.d
```

-	Created: Wed, 04 May 2016 03:09:18 GMT
-	Parent Layer: `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:4fc566a7c22ab414ecafcea1db51a7687bfff449c21fcba1ca3ffc8f7431fedc`
-	v2 Content-Length: 180.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:15 GMT

#### `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`

```dockerfile
RUN apt-get update && apt-get install -y apache2-bin apache2.2-common --no-install-recommends && rm -rf /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:19:10 GMT
-	Parent Layer: `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 MB (7144258 bytes)
-	v2 Blob: `sha256:b06a1bacee5136cb74c8d381a9edf716a54b0b7e968561171b16371fe2148e0e`
-	v2 Content-Length: 2.8 MB (2844067 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:11 GMT

#### `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`

```dockerfile
RUN rm -rf /var/www/html && mkdir -p /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html && chown -R www-data:www-data /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html
```

-	Created: Wed, 04 May 2016 03:19:12 GMT
-	Parent Layer: `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:c5fc21fb6c0950653e5db96e21275266c2d6725bd22fc72cc7f74a1334270a39`
-	v2 Content-Length: 321.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:05 GMT

#### `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`

```dockerfile
RUN a2dismod mpm_event && a2enmod mpm_prefork
```

-	Created: Wed, 04 May 2016 03:19:14 GMT
-	Parent Layer: `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`
-	Docker Version: 1.9.1
-	Virtual Size: 68.0 B
-	v2 Blob: `sha256:df319b61c8697392699262bcd17786b49f94b0d55adbccc35ca6ebc980cde386`
-	v2 Content-Length: 431.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:00 GMT

#### `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`

```dockerfile
RUN mv /etc/apache2/apache2.conf /etc/apache2/apache2.conf.dist && rm /etc/apache2/conf-enabled/* /etc/apache2/sites-enabled/*
```

-	Created: Wed, 04 May 2016 03:19:15 GMT
-	Parent Layer: `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 KB (7115 bytes)
-	v2 Blob: `sha256:f958e52674095ca585ddb3e453e794a14722b0a58a7cf46677b81452db55cb9b`
-	v2 Content-Length: 3.4 KB (3364 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:57 GMT

#### `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`

```dockerfile
COPY file:cd759b8d41f4b210d6ab9589edc3741a6aa46739a169e73608046d3df8cbadc7 in /etc/apache2/apache2.conf
```

-	Created: Wed, 04 May 2016 03:19:16 GMT
-	Parent Layer: `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`
-	Docker Version: 1.9.1
-	Virtual Size: 1.5 KB (1520 bytes)
-	v2 Blob: `sha256:b06010f04fa85bbea9ae802425f6e747bc4e48476f7a04daa1b6db8236319a51`
-	v2 Content-Length: 867.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:54 GMT

#### `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`

```dockerfile
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`

```dockerfile
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`

```dockerfile
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`

```dockerfile
ENV PHP_VERSION=5.6.21
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`

```dockerfile
ENV PHP_FILENAME=php-5.6.21.tar.xz
```

-	Created: Wed, 04 May 2016 03:54:09 GMT
-	Parent Layer: `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`

```dockerfile
ENV PHP_SHA256=566ff1a486cb0485ed477a91ea292423f77a58671270ff73b74e67e3ce7084f9
```

-	Created: Wed, 04 May 2016 03:54:10 GMT
-	Parent Layer: `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`

```dockerfile
RUN set -xe \
	&& buildDeps=" \
		$PHP_EXTRA_BUILD_DEPS \
		libcurl4-openssl-dev \
		libedit-dev \
		libsqlite3-dev \
		libssl-dev \
		libxml2-dev \
		xz-utils \
	" \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME/from/this/mirror" -o "$PHP_FILENAME" \
	&& echo "$PHP_SHA256 *$PHP_FILENAME" | sha256sum -c - \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME.asc/from/this/mirror" -o "$PHP_FILENAME.asc" \
	&& export GNUPGHOME="$(mktemp -d)" \
	&& for key in $GPG_KEYS; do \
		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; \
	done \
	&& gpg --batch --verify "$PHP_FILENAME.asc" "$PHP_FILENAME" \
	&& rm -r "$GNUPGHOME" "$PHP_FILENAME.asc" \
	&& mkdir -p /usr/src/php \
	&& tar -xf "$PHP_FILENAME" -C /usr/src/php --strip-components=1 \
	&& rm "$PHP_FILENAME" \
	&& cd /usr/src/php \
	&& ./configure \
		--with-config-file-path="$PHP_INI_DIR" \
		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" \
		$PHP_EXTRA_CONFIGURE_ARGS \
		--disable-cgi \
		--enable-mysqlnd \
		--enable-mbstring \
		--with-curl \
		--with-libedit \
		--with-openssl \
		--with-zlib \
	&& make -j"$(nproc)" \
	&& make install \
	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } \
	&& make clean \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps
```

-	Created: Wed, 04 May 2016 03:58:40 GMT
-	Parent Layer: `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`
-	Docker Version: 1.9.1
-	Virtual Size: 157.3 MB (157283614 bytes)
-	v2 Blob: `sha256:17c1b5f8acff40ea4896f49832dcb3603f88682db67cac65231ea688d2b5f096`
-	v2 Content-Length: 33.5 MB (33456893 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:38 GMT

#### `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`

```dockerfile
COPY multi:82b89724359b10e4fa6ed1d5d2d5ab38544995f1ed9288734f40288633831460 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:46 GMT
-	Parent Layer: `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`
-	Docker Version: 1.9.1
-	Virtual Size: 3.6 KB (3582 bytes)
-	v2 Blob: `sha256:2ed292d591c77a4a469bf3943d6b6b6bae8fd7db68447e2bd82295835fc541f7`
-	v2 Content-Length: 1.5 KB (1547 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:04 GMT

#### `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`

```dockerfile
COPY file:7f47595ed3e349ddf206e03fa4cceb50bbc7e82f815fcd7b924339356c688281 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:47 GMT
-	Parent Layer: `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`
-	Docker Version: 1.9.1
-	Virtual Size: 132.0 B
-	v2 Blob: `sha256:5ea0585ac6f234065af27594fc6ce67264271aec816eaf1f0eb5cdd92de79771`
-	v2 Content-Length: 291.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:01 GMT

#### `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`

```dockerfile
WORKDIR /var/www/html
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`

```dockerfile
EXPOSE 80/tcp
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Wed, 04 May 2016 03:58:49 GMT
-	Parent Layer: `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`

```dockerfile
RUN a2enmod rewrite expires
```

-	Created: Thu, 05 May 2016 05:59:49 GMT
-	Parent Layer: `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`
-	Docker Version: 1.9.1
-	Virtual Size: 60.0 B
-	v2 Blob: `sha256:f53bd09519680e814c527a086ebbdb79224f78b7ec18248570700f57287aac58`
-	v2 Content-Length: 325.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:35:05 GMT

#### `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`

```dockerfile
RUN apt-get update && apt-get install -y libpng12-dev libjpeg-dev && rm -rf /var/lib/apt/lists/* \
	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr \
	&& docker-php-ext-install gd mysqli opcache
```

-	Created: Thu, 05 May 2016 06:01:34 GMT
-	Parent Layer: `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`
-	Docker Version: 1.9.1
-	Virtual Size: 14.8 MB (14798027 bytes)
-	v2 Blob: `sha256:93949259a9c2121cd50bddbc28d3d01fae11cee18b3ff1c2ce1df5e90a11e6c9`
-	v2 Content-Length: 4.4 MB (4442966 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 23:35:02 GMT

#### `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`

```dockerfile
RUN { \
		echo 'opcache.memory_consumption=128'; \
		echo 'opcache.interned_strings_buffer=8'; \
		echo 'opcache.max_accelerated_files=4000'; \
		echo 'opcache.revalidate_freq=60'; \
		echo 'opcache.fast_shutdown=1'; \
		echo 'opcache.enable_cli=1'; \
	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
```

-	Created: Thu, 05 May 2016 06:01:36 GMT
-	Parent Layer: `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`
-	Docker Version: 1.9.1
-	Virtual Size: 172.0 B
-	v2 Blob: `sha256:33ea413bdf772998eccb0a0c97178f5e9b4568f46cfbd445fa47775b77e47928`
-	v2 Content-Length: 330.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:34:56 GMT

#### `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`

```dockerfile
VOLUME [/var/www/html]
```

-	Created: Thu, 05 May 2016 06:01:37 GMT
-	Parent Layer: `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`

```dockerfile
ENV WORDPRESS_VERSION=4.5.2
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`

```dockerfile
ENV WORDPRESS_SHA1=bab94003a5d2285f6ae76407e7b1bbb75382c36e
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`

```dockerfile
RUN curl -o wordpress.tar.gz -SL https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz \
	&& echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c - \
	&& tar -xzf wordpress.tar.gz -C /usr/src/ \
	&& rm wordpress.tar.gz \
	&& chown -R www-data:www-data /usr/src/wordpress
```

-	Created: Tue, 10 May 2016 01:26:05 GMT
-	Parent Layer: `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`
-	Docker Version: 1.9.1
-	Virtual Size: 21.9 MB (21908610 bytes)
-	v2 Blob: `sha256:8d937227258e1c2b37b6f1b004620ddc2a58b96d34ae75dc26c7a159d0f56bfc`
-	v2 Content-Length: 7.6 MB (7610147 bytes)
-	v2 Last-Modified: Tue, 10 May 2016 01:55:22 GMT

#### `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`

```dockerfile
COPY file:e4f27140dddd16cd34ce106cb7587b487bdf49693a3436dc23a89fcb0f933d05 in /entrypoint.sh
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`
-	Docker Version: 1.9.1
-	Virtual Size: 5.2 KB (5155 bytes)
-	v2 Blob: `sha256:f79a39a56bc213acb9b5131bb94562383aecb31e2c72086fafd6aa36a9617201`
-	v2 Content-Length: 2.5 KB (2492 bytes)
-	v2 Last-Modified: Thu, 12 May 2016 20:00:20 GMT

#### `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a913b4803726a52dfbf28eb4ad920a302ec4b09235cbc4de4bdb43fcab8d7abc`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Thu, 12 May 2016 19:21:00 GMT
-	Parent Layer: `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

## `wordpress:apache`

```console
$ docker pull library/wordpress@sha256:ae4764d10e755f9d7a106f33ceec0850636ab9f7fdd257e600dc9f98a6b1e4ac
```

-	Total Virtual Size: 520.7 MB (520660320 bytes)
-	Total v2 Content-Length: 177.1 MB (177107442 bytes)

### Layers (33)

#### `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`

```dockerfile
ADD file:dc2eddd5d35b9d66e4db747f5939b2be7f863dcee64c934b0da690f55a23aee8 in /
```

-	Created: Tue, 03 May 2016 20:57:39 GMT
-	Docker Version: 1.9.1
-	Virtual Size: 125.1 MB (125093399 bytes)
-	v2 Blob: `sha256:8b87079b7a06f9b72e3cca2c984c60e118229c60f0bff855d822f758c112b485`
-	v2 Content-Length: 51.4 MB (51355855 bytes)
-	v2 Last-Modified: Tue, 03 May 2016 20:59:55 GMT

#### `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Tue, 03 May 2016 20:57:42 GMT
-	Parent Layer: `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`

```dockerfile
RUN apt-get update && apt-get install -y \
		autoconf \
		file \
		g++ \
		gcc \
		libc-dev \
		make \
		pkg-config \
		re2c \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:08:29 GMT
-	Parent Layer: `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`
-	Docker Version: 1.9.1
-	Virtual Size: 177.8 MB (177788678 bytes)
-	v2 Blob: `sha256:af1704cb90e1fa3243238682e49412335aba819dc71452142be0a48851ba039a`
-	v2 Content-Length: 69.6 MB (69566346 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:08:02 GMT

#### `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`

```dockerfile
RUN apt-get update && apt-get install -y \
		ca-certificates \
		curl \
		libedit2 \
		libsqlite3-0 \
		libxml2 \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:09:15 GMT
-	Parent Layer: `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`
-	Docker Version: 1.9.1
-	Virtual Size: 16.6 MB (16625930 bytes)
-	v2 Blob: `sha256:6acdef7ebe13fb272b2fb6ac4879f5c815a6e97b34f8f7b46fb3408fddaa03eb`
-	v2 Content-Length: 7.8 MB (7820508 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:26 GMT

#### `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`

```dockerfile
ENV PHP_INI_DIR=/usr/local/etc/php
```

-	Created: Wed, 04 May 2016 03:09:16 GMT
-	Parent Layer: `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`

```dockerfile
RUN mkdir -p $PHP_INI_DIR/conf.d
```

-	Created: Wed, 04 May 2016 03:09:18 GMT
-	Parent Layer: `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:4fc566a7c22ab414ecafcea1db51a7687bfff449c21fcba1ca3ffc8f7431fedc`
-	v2 Content-Length: 180.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:15 GMT

#### `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`

```dockerfile
RUN apt-get update && apt-get install -y apache2-bin apache2.2-common --no-install-recommends && rm -rf /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:19:10 GMT
-	Parent Layer: `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 MB (7144258 bytes)
-	v2 Blob: `sha256:b06a1bacee5136cb74c8d381a9edf716a54b0b7e968561171b16371fe2148e0e`
-	v2 Content-Length: 2.8 MB (2844067 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:11 GMT

#### `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`

```dockerfile
RUN rm -rf /var/www/html && mkdir -p /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html && chown -R www-data:www-data /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html
```

-	Created: Wed, 04 May 2016 03:19:12 GMT
-	Parent Layer: `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:c5fc21fb6c0950653e5db96e21275266c2d6725bd22fc72cc7f74a1334270a39`
-	v2 Content-Length: 321.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:05 GMT

#### `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`

```dockerfile
RUN a2dismod mpm_event && a2enmod mpm_prefork
```

-	Created: Wed, 04 May 2016 03:19:14 GMT
-	Parent Layer: `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`
-	Docker Version: 1.9.1
-	Virtual Size: 68.0 B
-	v2 Blob: `sha256:df319b61c8697392699262bcd17786b49f94b0d55adbccc35ca6ebc980cde386`
-	v2 Content-Length: 431.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:00 GMT

#### `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`

```dockerfile
RUN mv /etc/apache2/apache2.conf /etc/apache2/apache2.conf.dist && rm /etc/apache2/conf-enabled/* /etc/apache2/sites-enabled/*
```

-	Created: Wed, 04 May 2016 03:19:15 GMT
-	Parent Layer: `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 KB (7115 bytes)
-	v2 Blob: `sha256:f958e52674095ca585ddb3e453e794a14722b0a58a7cf46677b81452db55cb9b`
-	v2 Content-Length: 3.4 KB (3364 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:57 GMT

#### `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`

```dockerfile
COPY file:cd759b8d41f4b210d6ab9589edc3741a6aa46739a169e73608046d3df8cbadc7 in /etc/apache2/apache2.conf
```

-	Created: Wed, 04 May 2016 03:19:16 GMT
-	Parent Layer: `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`
-	Docker Version: 1.9.1
-	Virtual Size: 1.5 KB (1520 bytes)
-	v2 Blob: `sha256:b06010f04fa85bbea9ae802425f6e747bc4e48476f7a04daa1b6db8236319a51`
-	v2 Content-Length: 867.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:54 GMT

#### `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`

```dockerfile
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`

```dockerfile
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`

```dockerfile
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`

```dockerfile
ENV PHP_VERSION=5.6.21
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`

```dockerfile
ENV PHP_FILENAME=php-5.6.21.tar.xz
```

-	Created: Wed, 04 May 2016 03:54:09 GMT
-	Parent Layer: `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`

```dockerfile
ENV PHP_SHA256=566ff1a486cb0485ed477a91ea292423f77a58671270ff73b74e67e3ce7084f9
```

-	Created: Wed, 04 May 2016 03:54:10 GMT
-	Parent Layer: `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`

```dockerfile
RUN set -xe \
	&& buildDeps=" \
		$PHP_EXTRA_BUILD_DEPS \
		libcurl4-openssl-dev \
		libedit-dev \
		libsqlite3-dev \
		libssl-dev \
		libxml2-dev \
		xz-utils \
	" \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME/from/this/mirror" -o "$PHP_FILENAME" \
	&& echo "$PHP_SHA256 *$PHP_FILENAME" | sha256sum -c - \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME.asc/from/this/mirror" -o "$PHP_FILENAME.asc" \
	&& export GNUPGHOME="$(mktemp -d)" \
	&& for key in $GPG_KEYS; do \
		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; \
	done \
	&& gpg --batch --verify "$PHP_FILENAME.asc" "$PHP_FILENAME" \
	&& rm -r "$GNUPGHOME" "$PHP_FILENAME.asc" \
	&& mkdir -p /usr/src/php \
	&& tar -xf "$PHP_FILENAME" -C /usr/src/php --strip-components=1 \
	&& rm "$PHP_FILENAME" \
	&& cd /usr/src/php \
	&& ./configure \
		--with-config-file-path="$PHP_INI_DIR" \
		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" \
		$PHP_EXTRA_CONFIGURE_ARGS \
		--disable-cgi \
		--enable-mysqlnd \
		--enable-mbstring \
		--with-curl \
		--with-libedit \
		--with-openssl \
		--with-zlib \
	&& make -j"$(nproc)" \
	&& make install \
	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } \
	&& make clean \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps
```

-	Created: Wed, 04 May 2016 03:58:40 GMT
-	Parent Layer: `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`
-	Docker Version: 1.9.1
-	Virtual Size: 157.3 MB (157283614 bytes)
-	v2 Blob: `sha256:17c1b5f8acff40ea4896f49832dcb3603f88682db67cac65231ea688d2b5f096`
-	v2 Content-Length: 33.5 MB (33456893 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:38 GMT

#### `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`

```dockerfile
COPY multi:82b89724359b10e4fa6ed1d5d2d5ab38544995f1ed9288734f40288633831460 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:46 GMT
-	Parent Layer: `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`
-	Docker Version: 1.9.1
-	Virtual Size: 3.6 KB (3582 bytes)
-	v2 Blob: `sha256:2ed292d591c77a4a469bf3943d6b6b6bae8fd7db68447e2bd82295835fc541f7`
-	v2 Content-Length: 1.5 KB (1547 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:04 GMT

#### `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`

```dockerfile
COPY file:7f47595ed3e349ddf206e03fa4cceb50bbc7e82f815fcd7b924339356c688281 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:47 GMT
-	Parent Layer: `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`
-	Docker Version: 1.9.1
-	Virtual Size: 132.0 B
-	v2 Blob: `sha256:5ea0585ac6f234065af27594fc6ce67264271aec816eaf1f0eb5cdd92de79771`
-	v2 Content-Length: 291.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:01 GMT

#### `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`

```dockerfile
WORKDIR /var/www/html
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`

```dockerfile
EXPOSE 80/tcp
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Wed, 04 May 2016 03:58:49 GMT
-	Parent Layer: `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`

```dockerfile
RUN a2enmod rewrite expires
```

-	Created: Thu, 05 May 2016 05:59:49 GMT
-	Parent Layer: `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`
-	Docker Version: 1.9.1
-	Virtual Size: 60.0 B
-	v2 Blob: `sha256:f53bd09519680e814c527a086ebbdb79224f78b7ec18248570700f57287aac58`
-	v2 Content-Length: 325.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:35:05 GMT

#### `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`

```dockerfile
RUN apt-get update && apt-get install -y libpng12-dev libjpeg-dev && rm -rf /var/lib/apt/lists/* \
	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr \
	&& docker-php-ext-install gd mysqli opcache
```

-	Created: Thu, 05 May 2016 06:01:34 GMT
-	Parent Layer: `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`
-	Docker Version: 1.9.1
-	Virtual Size: 14.8 MB (14798027 bytes)
-	v2 Blob: `sha256:93949259a9c2121cd50bddbc28d3d01fae11cee18b3ff1c2ce1df5e90a11e6c9`
-	v2 Content-Length: 4.4 MB (4442966 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 23:35:02 GMT

#### `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`

```dockerfile
RUN { \
		echo 'opcache.memory_consumption=128'; \
		echo 'opcache.interned_strings_buffer=8'; \
		echo 'opcache.max_accelerated_files=4000'; \
		echo 'opcache.revalidate_freq=60'; \
		echo 'opcache.fast_shutdown=1'; \
		echo 'opcache.enable_cli=1'; \
	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
```

-	Created: Thu, 05 May 2016 06:01:36 GMT
-	Parent Layer: `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`
-	Docker Version: 1.9.1
-	Virtual Size: 172.0 B
-	v2 Blob: `sha256:33ea413bdf772998eccb0a0c97178f5e9b4568f46cfbd445fa47775b77e47928`
-	v2 Content-Length: 330.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:34:56 GMT

#### `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`

```dockerfile
VOLUME [/var/www/html]
```

-	Created: Thu, 05 May 2016 06:01:37 GMT
-	Parent Layer: `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`

```dockerfile
ENV WORDPRESS_VERSION=4.5.2
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`

```dockerfile
ENV WORDPRESS_SHA1=bab94003a5d2285f6ae76407e7b1bbb75382c36e
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`

```dockerfile
RUN curl -o wordpress.tar.gz -SL https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz \
	&& echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c - \
	&& tar -xzf wordpress.tar.gz -C /usr/src/ \
	&& rm wordpress.tar.gz \
	&& chown -R www-data:www-data /usr/src/wordpress
```

-	Created: Tue, 10 May 2016 01:26:05 GMT
-	Parent Layer: `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`
-	Docker Version: 1.9.1
-	Virtual Size: 21.9 MB (21908610 bytes)
-	v2 Blob: `sha256:8d937227258e1c2b37b6f1b004620ddc2a58b96d34ae75dc26c7a159d0f56bfc`
-	v2 Content-Length: 7.6 MB (7610147 bytes)
-	v2 Last-Modified: Tue, 10 May 2016 01:55:22 GMT

#### `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`

```dockerfile
COPY file:e4f27140dddd16cd34ce106cb7587b487bdf49693a3436dc23a89fcb0f933d05 in /entrypoint.sh
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`
-	Docker Version: 1.9.1
-	Virtual Size: 5.2 KB (5155 bytes)
-	v2 Blob: `sha256:f79a39a56bc213acb9b5131bb94562383aecb31e2c72086fafd6aa36a9617201`
-	v2 Content-Length: 2.5 KB (2492 bytes)
-	v2 Last-Modified: Thu, 12 May 2016 20:00:20 GMT

#### `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a913b4803726a52dfbf28eb4ad920a302ec4b09235cbc4de4bdb43fcab8d7abc`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Thu, 12 May 2016 19:21:00 GMT
-	Parent Layer: `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

## `wordpress:4`

```console
$ docker pull library/wordpress@sha256:addcedb048f5599349c43730117c1d9d07fb83919822dfd964a3c2b3962e5aa3
```

-	Total Virtual Size: 520.7 MB (520660320 bytes)
-	Total v2 Content-Length: 177.1 MB (177107442 bytes)

### Layers (33)

#### `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`

```dockerfile
ADD file:dc2eddd5d35b9d66e4db747f5939b2be7f863dcee64c934b0da690f55a23aee8 in /
```

-	Created: Tue, 03 May 2016 20:57:39 GMT
-	Docker Version: 1.9.1
-	Virtual Size: 125.1 MB (125093399 bytes)
-	v2 Blob: `sha256:8b87079b7a06f9b72e3cca2c984c60e118229c60f0bff855d822f758c112b485`
-	v2 Content-Length: 51.4 MB (51355855 bytes)
-	v2 Last-Modified: Tue, 03 May 2016 20:59:55 GMT

#### `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Tue, 03 May 2016 20:57:42 GMT
-	Parent Layer: `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`

```dockerfile
RUN apt-get update && apt-get install -y \
		autoconf \
		file \
		g++ \
		gcc \
		libc-dev \
		make \
		pkg-config \
		re2c \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:08:29 GMT
-	Parent Layer: `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`
-	Docker Version: 1.9.1
-	Virtual Size: 177.8 MB (177788678 bytes)
-	v2 Blob: `sha256:af1704cb90e1fa3243238682e49412335aba819dc71452142be0a48851ba039a`
-	v2 Content-Length: 69.6 MB (69566346 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:08:02 GMT

#### `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`

```dockerfile
RUN apt-get update && apt-get install -y \
		ca-certificates \
		curl \
		libedit2 \
		libsqlite3-0 \
		libxml2 \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:09:15 GMT
-	Parent Layer: `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`
-	Docker Version: 1.9.1
-	Virtual Size: 16.6 MB (16625930 bytes)
-	v2 Blob: `sha256:6acdef7ebe13fb272b2fb6ac4879f5c815a6e97b34f8f7b46fb3408fddaa03eb`
-	v2 Content-Length: 7.8 MB (7820508 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:26 GMT

#### `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`

```dockerfile
ENV PHP_INI_DIR=/usr/local/etc/php
```

-	Created: Wed, 04 May 2016 03:09:16 GMT
-	Parent Layer: `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`

```dockerfile
RUN mkdir -p $PHP_INI_DIR/conf.d
```

-	Created: Wed, 04 May 2016 03:09:18 GMT
-	Parent Layer: `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:4fc566a7c22ab414ecafcea1db51a7687bfff449c21fcba1ca3ffc8f7431fedc`
-	v2 Content-Length: 180.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:15 GMT

#### `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`

```dockerfile
RUN apt-get update && apt-get install -y apache2-bin apache2.2-common --no-install-recommends && rm -rf /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:19:10 GMT
-	Parent Layer: `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 MB (7144258 bytes)
-	v2 Blob: `sha256:b06a1bacee5136cb74c8d381a9edf716a54b0b7e968561171b16371fe2148e0e`
-	v2 Content-Length: 2.8 MB (2844067 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:11 GMT

#### `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`

```dockerfile
RUN rm -rf /var/www/html && mkdir -p /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html && chown -R www-data:www-data /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html
```

-	Created: Wed, 04 May 2016 03:19:12 GMT
-	Parent Layer: `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:c5fc21fb6c0950653e5db96e21275266c2d6725bd22fc72cc7f74a1334270a39`
-	v2 Content-Length: 321.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:05 GMT

#### `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`

```dockerfile
RUN a2dismod mpm_event && a2enmod mpm_prefork
```

-	Created: Wed, 04 May 2016 03:19:14 GMT
-	Parent Layer: `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`
-	Docker Version: 1.9.1
-	Virtual Size: 68.0 B
-	v2 Blob: `sha256:df319b61c8697392699262bcd17786b49f94b0d55adbccc35ca6ebc980cde386`
-	v2 Content-Length: 431.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:00 GMT

#### `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`

```dockerfile
RUN mv /etc/apache2/apache2.conf /etc/apache2/apache2.conf.dist && rm /etc/apache2/conf-enabled/* /etc/apache2/sites-enabled/*
```

-	Created: Wed, 04 May 2016 03:19:15 GMT
-	Parent Layer: `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 KB (7115 bytes)
-	v2 Blob: `sha256:f958e52674095ca585ddb3e453e794a14722b0a58a7cf46677b81452db55cb9b`
-	v2 Content-Length: 3.4 KB (3364 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:57 GMT

#### `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`

```dockerfile
COPY file:cd759b8d41f4b210d6ab9589edc3741a6aa46739a169e73608046d3df8cbadc7 in /etc/apache2/apache2.conf
```

-	Created: Wed, 04 May 2016 03:19:16 GMT
-	Parent Layer: `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`
-	Docker Version: 1.9.1
-	Virtual Size: 1.5 KB (1520 bytes)
-	v2 Blob: `sha256:b06010f04fa85bbea9ae802425f6e747bc4e48476f7a04daa1b6db8236319a51`
-	v2 Content-Length: 867.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:54 GMT

#### `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`

```dockerfile
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`

```dockerfile
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`

```dockerfile
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`

```dockerfile
ENV PHP_VERSION=5.6.21
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`

```dockerfile
ENV PHP_FILENAME=php-5.6.21.tar.xz
```

-	Created: Wed, 04 May 2016 03:54:09 GMT
-	Parent Layer: `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`

```dockerfile
ENV PHP_SHA256=566ff1a486cb0485ed477a91ea292423f77a58671270ff73b74e67e3ce7084f9
```

-	Created: Wed, 04 May 2016 03:54:10 GMT
-	Parent Layer: `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`

```dockerfile
RUN set -xe \
	&& buildDeps=" \
		$PHP_EXTRA_BUILD_DEPS \
		libcurl4-openssl-dev \
		libedit-dev \
		libsqlite3-dev \
		libssl-dev \
		libxml2-dev \
		xz-utils \
	" \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME/from/this/mirror" -o "$PHP_FILENAME" \
	&& echo "$PHP_SHA256 *$PHP_FILENAME" | sha256sum -c - \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME.asc/from/this/mirror" -o "$PHP_FILENAME.asc" \
	&& export GNUPGHOME="$(mktemp -d)" \
	&& for key in $GPG_KEYS; do \
		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; \
	done \
	&& gpg --batch --verify "$PHP_FILENAME.asc" "$PHP_FILENAME" \
	&& rm -r "$GNUPGHOME" "$PHP_FILENAME.asc" \
	&& mkdir -p /usr/src/php \
	&& tar -xf "$PHP_FILENAME" -C /usr/src/php --strip-components=1 \
	&& rm "$PHP_FILENAME" \
	&& cd /usr/src/php \
	&& ./configure \
		--with-config-file-path="$PHP_INI_DIR" \
		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" \
		$PHP_EXTRA_CONFIGURE_ARGS \
		--disable-cgi \
		--enable-mysqlnd \
		--enable-mbstring \
		--with-curl \
		--with-libedit \
		--with-openssl \
		--with-zlib \
	&& make -j"$(nproc)" \
	&& make install \
	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } \
	&& make clean \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps
```

-	Created: Wed, 04 May 2016 03:58:40 GMT
-	Parent Layer: `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`
-	Docker Version: 1.9.1
-	Virtual Size: 157.3 MB (157283614 bytes)
-	v2 Blob: `sha256:17c1b5f8acff40ea4896f49832dcb3603f88682db67cac65231ea688d2b5f096`
-	v2 Content-Length: 33.5 MB (33456893 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:38 GMT

#### `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`

```dockerfile
COPY multi:82b89724359b10e4fa6ed1d5d2d5ab38544995f1ed9288734f40288633831460 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:46 GMT
-	Parent Layer: `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`
-	Docker Version: 1.9.1
-	Virtual Size: 3.6 KB (3582 bytes)
-	v2 Blob: `sha256:2ed292d591c77a4a469bf3943d6b6b6bae8fd7db68447e2bd82295835fc541f7`
-	v2 Content-Length: 1.5 KB (1547 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:04 GMT

#### `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`

```dockerfile
COPY file:7f47595ed3e349ddf206e03fa4cceb50bbc7e82f815fcd7b924339356c688281 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:47 GMT
-	Parent Layer: `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`
-	Docker Version: 1.9.1
-	Virtual Size: 132.0 B
-	v2 Blob: `sha256:5ea0585ac6f234065af27594fc6ce67264271aec816eaf1f0eb5cdd92de79771`
-	v2 Content-Length: 291.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:01 GMT

#### `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`

```dockerfile
WORKDIR /var/www/html
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`

```dockerfile
EXPOSE 80/tcp
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Wed, 04 May 2016 03:58:49 GMT
-	Parent Layer: `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`

```dockerfile
RUN a2enmod rewrite expires
```

-	Created: Thu, 05 May 2016 05:59:49 GMT
-	Parent Layer: `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`
-	Docker Version: 1.9.1
-	Virtual Size: 60.0 B
-	v2 Blob: `sha256:f53bd09519680e814c527a086ebbdb79224f78b7ec18248570700f57287aac58`
-	v2 Content-Length: 325.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:35:05 GMT

#### `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`

```dockerfile
RUN apt-get update && apt-get install -y libpng12-dev libjpeg-dev && rm -rf /var/lib/apt/lists/* \
	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr \
	&& docker-php-ext-install gd mysqli opcache
```

-	Created: Thu, 05 May 2016 06:01:34 GMT
-	Parent Layer: `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`
-	Docker Version: 1.9.1
-	Virtual Size: 14.8 MB (14798027 bytes)
-	v2 Blob: `sha256:93949259a9c2121cd50bddbc28d3d01fae11cee18b3ff1c2ce1df5e90a11e6c9`
-	v2 Content-Length: 4.4 MB (4442966 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 23:35:02 GMT

#### `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`

```dockerfile
RUN { \
		echo 'opcache.memory_consumption=128'; \
		echo 'opcache.interned_strings_buffer=8'; \
		echo 'opcache.max_accelerated_files=4000'; \
		echo 'opcache.revalidate_freq=60'; \
		echo 'opcache.fast_shutdown=1'; \
		echo 'opcache.enable_cli=1'; \
	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
```

-	Created: Thu, 05 May 2016 06:01:36 GMT
-	Parent Layer: `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`
-	Docker Version: 1.9.1
-	Virtual Size: 172.0 B
-	v2 Blob: `sha256:33ea413bdf772998eccb0a0c97178f5e9b4568f46cfbd445fa47775b77e47928`
-	v2 Content-Length: 330.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:34:56 GMT

#### `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`

```dockerfile
VOLUME [/var/www/html]
```

-	Created: Thu, 05 May 2016 06:01:37 GMT
-	Parent Layer: `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`

```dockerfile
ENV WORDPRESS_VERSION=4.5.2
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`

```dockerfile
ENV WORDPRESS_SHA1=bab94003a5d2285f6ae76407e7b1bbb75382c36e
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`

```dockerfile
RUN curl -o wordpress.tar.gz -SL https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz \
	&& echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c - \
	&& tar -xzf wordpress.tar.gz -C /usr/src/ \
	&& rm wordpress.tar.gz \
	&& chown -R www-data:www-data /usr/src/wordpress
```

-	Created: Tue, 10 May 2016 01:26:05 GMT
-	Parent Layer: `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`
-	Docker Version: 1.9.1
-	Virtual Size: 21.9 MB (21908610 bytes)
-	v2 Blob: `sha256:8d937227258e1c2b37b6f1b004620ddc2a58b96d34ae75dc26c7a159d0f56bfc`
-	v2 Content-Length: 7.6 MB (7610147 bytes)
-	v2 Last-Modified: Tue, 10 May 2016 01:55:22 GMT

#### `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`

```dockerfile
COPY file:e4f27140dddd16cd34ce106cb7587b487bdf49693a3436dc23a89fcb0f933d05 in /entrypoint.sh
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`
-	Docker Version: 1.9.1
-	Virtual Size: 5.2 KB (5155 bytes)
-	v2 Blob: `sha256:f79a39a56bc213acb9b5131bb94562383aecb31e2c72086fafd6aa36a9617201`
-	v2 Content-Length: 2.5 KB (2492 bytes)
-	v2 Last-Modified: Thu, 12 May 2016 20:00:20 GMT

#### `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a913b4803726a52dfbf28eb4ad920a302ec4b09235cbc4de4bdb43fcab8d7abc`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Thu, 12 May 2016 19:21:00 GMT
-	Parent Layer: `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

## `wordpress:latest`

```console
$ docker pull library/wordpress@sha256:0ee9d65c19b39496363224c8b6ff0dc25dda8f71b8aabc24662a552e6ed0443d
```

-	Total Virtual Size: 520.7 MB (520660320 bytes)
-	Total v2 Content-Length: 177.1 MB (177107442 bytes)

### Layers (33)

#### `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`

```dockerfile
ADD file:dc2eddd5d35b9d66e4db747f5939b2be7f863dcee64c934b0da690f55a23aee8 in /
```

-	Created: Tue, 03 May 2016 20:57:39 GMT
-	Docker Version: 1.9.1
-	Virtual Size: 125.1 MB (125093399 bytes)
-	v2 Blob: `sha256:8b87079b7a06f9b72e3cca2c984c60e118229c60f0bff855d822f758c112b485`
-	v2 Content-Length: 51.4 MB (51355855 bytes)
-	v2 Last-Modified: Tue, 03 May 2016 20:59:55 GMT

#### `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Tue, 03 May 2016 20:57:42 GMT
-	Parent Layer: `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`

```dockerfile
RUN apt-get update && apt-get install -y \
		autoconf \
		file \
		g++ \
		gcc \
		libc-dev \
		make \
		pkg-config \
		re2c \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:08:29 GMT
-	Parent Layer: `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`
-	Docker Version: 1.9.1
-	Virtual Size: 177.8 MB (177788678 bytes)
-	v2 Blob: `sha256:af1704cb90e1fa3243238682e49412335aba819dc71452142be0a48851ba039a`
-	v2 Content-Length: 69.6 MB (69566346 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:08:02 GMT

#### `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`

```dockerfile
RUN apt-get update && apt-get install -y \
		ca-certificates \
		curl \
		libedit2 \
		libsqlite3-0 \
		libxml2 \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:09:15 GMT
-	Parent Layer: `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`
-	Docker Version: 1.9.1
-	Virtual Size: 16.6 MB (16625930 bytes)
-	v2 Blob: `sha256:6acdef7ebe13fb272b2fb6ac4879f5c815a6e97b34f8f7b46fb3408fddaa03eb`
-	v2 Content-Length: 7.8 MB (7820508 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:26 GMT

#### `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`

```dockerfile
ENV PHP_INI_DIR=/usr/local/etc/php
```

-	Created: Wed, 04 May 2016 03:09:16 GMT
-	Parent Layer: `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`

```dockerfile
RUN mkdir -p $PHP_INI_DIR/conf.d
```

-	Created: Wed, 04 May 2016 03:09:18 GMT
-	Parent Layer: `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:4fc566a7c22ab414ecafcea1db51a7687bfff449c21fcba1ca3ffc8f7431fedc`
-	v2 Content-Length: 180.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:15 GMT

#### `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`

```dockerfile
RUN apt-get update && apt-get install -y apache2-bin apache2.2-common --no-install-recommends && rm -rf /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:19:10 GMT
-	Parent Layer: `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 MB (7144258 bytes)
-	v2 Blob: `sha256:b06a1bacee5136cb74c8d381a9edf716a54b0b7e968561171b16371fe2148e0e`
-	v2 Content-Length: 2.8 MB (2844067 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:11 GMT

#### `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`

```dockerfile
RUN rm -rf /var/www/html && mkdir -p /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html && chown -R www-data:www-data /var/lock/apache2 /var/run/apache2 /var/log/apache2 /var/www/html
```

-	Created: Wed, 04 May 2016 03:19:12 GMT
-	Parent Layer: `a7446855261994b84f0310de5e34c52f57e4d857dfa1473c67618b1ecc572764`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:c5fc21fb6c0950653e5db96e21275266c2d6725bd22fc72cc7f74a1334270a39`
-	v2 Content-Length: 321.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:05 GMT

#### `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`

```dockerfile
RUN a2dismod mpm_event && a2enmod mpm_prefork
```

-	Created: Wed, 04 May 2016 03:19:14 GMT
-	Parent Layer: `e4dd3bdcf90ced3976f97149467fa626317e84cb30c2774fe05aaa4e662fac6d`
-	Docker Version: 1.9.1
-	Virtual Size: 68.0 B
-	v2 Blob: `sha256:df319b61c8697392699262bcd17786b49f94b0d55adbccc35ca6ebc980cde386`
-	v2 Content-Length: 431.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:00 GMT

#### `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`

```dockerfile
RUN mv /etc/apache2/apache2.conf /etc/apache2/apache2.conf.dist && rm /etc/apache2/conf-enabled/* /etc/apache2/sites-enabled/*
```

-	Created: Wed, 04 May 2016 03:19:15 GMT
-	Parent Layer: `42b784d01ef8310dd1d1a04fe2fffc116a92c76bcf64a96edfc9b542a31e4a2a`
-	Docker Version: 1.9.1
-	Virtual Size: 7.1 KB (7115 bytes)
-	v2 Blob: `sha256:f958e52674095ca585ddb3e453e794a14722b0a58a7cf46677b81452db55cb9b`
-	v2 Content-Length: 3.4 KB (3364 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:57 GMT

#### `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`

```dockerfile
COPY file:cd759b8d41f4b210d6ab9589edc3741a6aa46739a169e73608046d3df8cbadc7 in /etc/apache2/apache2.conf
```

-	Created: Wed, 04 May 2016 03:19:16 GMT
-	Parent Layer: `bcfb9ae27143275b33db263a87a1b4b772db737040de74201a3ab5e1bcbe6bd1`
-	Docker Version: 1.9.1
-	Virtual Size: 1.5 KB (1520 bytes)
-	v2 Blob: `sha256:b06010f04fa85bbea9ae802425f6e747bc4e48476f7a04daa1b6db8236319a51`
-	v2 Content-Length: 867.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:54 GMT

#### `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`

```dockerfile
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `c8271b6eea837bc865847ce4429afa45e5a543ad1ab655abbac7bb8130347cd4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`

```dockerfile
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
```

-	Created: Wed, 04 May 2016 03:19:17 GMT
-	Parent Layer: `bb1ef3989406d99b4bcb7525cb832485545f843c4488ba677ac95441e8b545f9`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`

```dockerfile
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `a6ce5d6587c45110b90316cdb386ff3f46477a286fc320e3636ad3c221075255`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`

```dockerfile
ENV PHP_VERSION=5.6.21
```

-	Created: Wed, 04 May 2016 03:54:08 GMT
-	Parent Layer: `c5eece3427396516f6751e4b7dad263f7a001e23fa23419d1d952b248302bd82`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`

```dockerfile
ENV PHP_FILENAME=php-5.6.21.tar.xz
```

-	Created: Wed, 04 May 2016 03:54:09 GMT
-	Parent Layer: `a022608ab2ce9cac78e4652c197466575f725a8c051177e32edda82edf384b06`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`

```dockerfile
ENV PHP_SHA256=566ff1a486cb0485ed477a91ea292423f77a58671270ff73b74e67e3ce7084f9
```

-	Created: Wed, 04 May 2016 03:54:10 GMT
-	Parent Layer: `8639a9b849f90438463cee838c91c390852586d0f9dc0c9755711bc2e041dac4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`

```dockerfile
RUN set -xe \
	&& buildDeps=" \
		$PHP_EXTRA_BUILD_DEPS \
		libcurl4-openssl-dev \
		libedit-dev \
		libsqlite3-dev \
		libssl-dev \
		libxml2-dev \
		xz-utils \
	" \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME/from/this/mirror" -o "$PHP_FILENAME" \
	&& echo "$PHP_SHA256 *$PHP_FILENAME" | sha256sum -c - \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME.asc/from/this/mirror" -o "$PHP_FILENAME.asc" \
	&& export GNUPGHOME="$(mktemp -d)" \
	&& for key in $GPG_KEYS; do \
		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; \
	done \
	&& gpg --batch --verify "$PHP_FILENAME.asc" "$PHP_FILENAME" \
	&& rm -r "$GNUPGHOME" "$PHP_FILENAME.asc" \
	&& mkdir -p /usr/src/php \
	&& tar -xf "$PHP_FILENAME" -C /usr/src/php --strip-components=1 \
	&& rm "$PHP_FILENAME" \
	&& cd /usr/src/php \
	&& ./configure \
		--with-config-file-path="$PHP_INI_DIR" \
		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" \
		$PHP_EXTRA_CONFIGURE_ARGS \
		--disable-cgi \
		--enable-mysqlnd \
		--enable-mbstring \
		--with-curl \
		--with-libedit \
		--with-openssl \
		--with-zlib \
	&& make -j"$(nproc)" \
	&& make install \
	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } \
	&& make clean \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps
```

-	Created: Wed, 04 May 2016 03:58:40 GMT
-	Parent Layer: `a8d5c98d79b098a794930fedf8fc611999f2dc11b2ba69b50bef51afd39daf63`
-	Docker Version: 1.9.1
-	Virtual Size: 157.3 MB (157283614 bytes)
-	v2 Blob: `sha256:17c1b5f8acff40ea4896f49832dcb3603f88682db67cac65231ea688d2b5f096`
-	v2 Content-Length: 33.5 MB (33456893 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:38 GMT

#### `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`

```dockerfile
COPY multi:82b89724359b10e4fa6ed1d5d2d5ab38544995f1ed9288734f40288633831460 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:46 GMT
-	Parent Layer: `7b12ed764531e12bf23ee5e2918dfcb79fbbc2906f7314a563612b6a5f4fa35a`
-	Docker Version: 1.9.1
-	Virtual Size: 3.6 KB (3582 bytes)
-	v2 Blob: `sha256:2ed292d591c77a4a469bf3943d6b6b6bae8fd7db68447e2bd82295835fc541f7`
-	v2 Content-Length: 1.5 KB (1547 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:06:04 GMT

#### `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`

```dockerfile
COPY file:7f47595ed3e349ddf206e03fa4cceb50bbc7e82f815fcd7b924339356c688281 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 03:58:47 GMT
-	Parent Layer: `5919992a1dd2bd39d84d13c114ad6e521330e952b11e41877c98fdd289c4e331`
-	Docker Version: 1.9.1
-	Virtual Size: 132.0 B
-	v2 Blob: `sha256:5ea0585ac6f234065af27594fc6ce67264271aec816eaf1f0eb5cdd92de79771`
-	v2 Content-Length: 291.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:06:01 GMT

#### `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`

```dockerfile
WORKDIR /var/www/html
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `b77eb22ebe756f22da5210d38d93bc6f7045f3184a3e29c50d17c221ff4c8d9e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`

```dockerfile
EXPOSE 80/tcp
```

-	Created: Wed, 04 May 2016 03:58:48 GMT
-	Parent Layer: `fec68a4814ab55120be56d65fc38c3e951be00798247c1661169ef72b24cc6fc`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Wed, 04 May 2016 03:58:49 GMT
-	Parent Layer: `31e69d457ab8cca903fbdc86a0908b71b65fa5f60c21f00234b4ed22db33e296`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`

```dockerfile
RUN a2enmod rewrite expires
```

-	Created: Thu, 05 May 2016 05:59:49 GMT
-	Parent Layer: `10e778c86cabf0ac20ace4e48bb32bacaa9b8eea3fe3fd4fc44d6b2d694d8283`
-	Docker Version: 1.9.1
-	Virtual Size: 60.0 B
-	v2 Blob: `sha256:f53bd09519680e814c527a086ebbdb79224f78b7ec18248570700f57287aac58`
-	v2 Content-Length: 325.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:35:05 GMT

#### `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`

```dockerfile
RUN apt-get update && apt-get install -y libpng12-dev libjpeg-dev && rm -rf /var/lib/apt/lists/* \
	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr \
	&& docker-php-ext-install gd mysqli opcache
```

-	Created: Thu, 05 May 2016 06:01:34 GMT
-	Parent Layer: `e9969f9705dd5a7b871923922d270239703a0350f3d23e7cdca9ed29fcc07029`
-	Docker Version: 1.9.1
-	Virtual Size: 14.8 MB (14798027 bytes)
-	v2 Blob: `sha256:93949259a9c2121cd50bddbc28d3d01fae11cee18b3ff1c2ce1df5e90a11e6c9`
-	v2 Content-Length: 4.4 MB (4442966 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 23:35:02 GMT

#### `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`

```dockerfile
RUN { \
		echo 'opcache.memory_consumption=128'; \
		echo 'opcache.interned_strings_buffer=8'; \
		echo 'opcache.max_accelerated_files=4000'; \
		echo 'opcache.revalidate_freq=60'; \
		echo 'opcache.fast_shutdown=1'; \
		echo 'opcache.enable_cli=1'; \
	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
```

-	Created: Thu, 05 May 2016 06:01:36 GMT
-	Parent Layer: `2aefed34d6dd6c28ad3268fd1f9822ca1e752de2f472fa49c63d07448bb5464b`
-	Docker Version: 1.9.1
-	Virtual Size: 172.0 B
-	v2 Blob: `sha256:33ea413bdf772998eccb0a0c97178f5e9b4568f46cfbd445fa47775b77e47928`
-	v2 Content-Length: 330.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:34:56 GMT

#### `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`

```dockerfile
VOLUME [/var/www/html]
```

-	Created: Thu, 05 May 2016 06:01:37 GMT
-	Parent Layer: `567c6e3cca7480e42cec7847cb66fc91702fc3613791f159d3c489e449dba5c7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`

```dockerfile
ENV WORDPRESS_VERSION=4.5.2
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `d4ad855c03a508f23de79864b8f5bf6d0966b7dbd7f8c0bf608568d30b504b0e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`

```dockerfile
ENV WORDPRESS_SHA1=bab94003a5d2285f6ae76407e7b1bbb75382c36e
```

-	Created: Tue, 10 May 2016 01:26:03 GMT
-	Parent Layer: `f77f965e3e2c5ad0cfac706e3d4b300c7a06b685434e3786c50b095dde236916`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`

```dockerfile
RUN curl -o wordpress.tar.gz -SL https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz \
	&& echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c - \
	&& tar -xzf wordpress.tar.gz -C /usr/src/ \
	&& rm wordpress.tar.gz \
	&& chown -R www-data:www-data /usr/src/wordpress
```

-	Created: Tue, 10 May 2016 01:26:05 GMT
-	Parent Layer: `665a6505e915b469eef92c98e2cb6464c438bb0299f2d5aae747f13f0fbd9fae`
-	Docker Version: 1.9.1
-	Virtual Size: 21.9 MB (21908610 bytes)
-	v2 Blob: `sha256:8d937227258e1c2b37b6f1b004620ddc2a58b96d34ae75dc26c7a159d0f56bfc`
-	v2 Content-Length: 7.6 MB (7610147 bytes)
-	v2 Last-Modified: Tue, 10 May 2016 01:55:22 GMT

#### `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`

```dockerfile
COPY file:e4f27140dddd16cd34ce106cb7587b487bdf49693a3436dc23a89fcb0f933d05 in /entrypoint.sh
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `71e43e6e65be93d57621eac7719abca0919d987d6a976cd0f270f77823d33c7f`
-	Docker Version: 1.9.1
-	Virtual Size: 5.2 KB (5155 bytes)
-	v2 Blob: `sha256:f79a39a56bc213acb9b5131bb94562383aecb31e2c72086fafd6aa36a9617201`
-	v2 Content-Length: 2.5 KB (2492 bytes)
-	v2 Last-Modified: Thu, 12 May 2016 20:00:20 GMT

#### `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Thu, 12 May 2016 19:20:59 GMT
-	Parent Layer: `d15fddd154754ef0b0153abb61faeaef0e4eabd120dde72ee126e55d3c46b133`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `a913b4803726a52dfbf28eb4ad920a302ec4b09235cbc4de4bdb43fcab8d7abc`

```dockerfile
CMD ["apache2-foreground"]
```

-	Created: Thu, 12 May 2016 19:21:00 GMT
-	Parent Layer: `e290738480e29a7ead619baf74272e7eb440ecfc591d3b79d9ed190ad3ed6c13`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

## `wordpress:4.5.2-fpm`

```console
$ docker pull library/wordpress@sha256:d4efacf10ae2ab14130f2115f067e7f92955a1fa42b4f568368dd229691631bd
```

-	Total Virtual Size: 492.4 MB (492434366 bytes)
-	Total v2 Content-Length: 167.3 MB (167260138 bytes)

### Layers (26)

#### `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`

```dockerfile
ADD file:dc2eddd5d35b9d66e4db747f5939b2be7f863dcee64c934b0da690f55a23aee8 in /
```

-	Created: Tue, 03 May 2016 20:57:39 GMT
-	Docker Version: 1.9.1
-	Virtual Size: 125.1 MB (125093399 bytes)
-	v2 Blob: `sha256:8b87079b7a06f9b72e3cca2c984c60e118229c60f0bff855d822f758c112b485`
-	v2 Content-Length: 51.4 MB (51355855 bytes)
-	v2 Last-Modified: Tue, 03 May 2016 20:59:55 GMT

#### `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Tue, 03 May 2016 20:57:42 GMT
-	Parent Layer: `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`

```dockerfile
RUN apt-get update && apt-get install -y \
		autoconf \
		file \
		g++ \
		gcc \
		libc-dev \
		make \
		pkg-config \
		re2c \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:08:29 GMT
-	Parent Layer: `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`
-	Docker Version: 1.9.1
-	Virtual Size: 177.8 MB (177788678 bytes)
-	v2 Blob: `sha256:af1704cb90e1fa3243238682e49412335aba819dc71452142be0a48851ba039a`
-	v2 Content-Length: 69.6 MB (69566346 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:08:02 GMT

#### `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`

```dockerfile
RUN apt-get update && apt-get install -y \
		ca-certificates \
		curl \
		libedit2 \
		libsqlite3-0 \
		libxml2 \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:09:15 GMT
-	Parent Layer: `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`
-	Docker Version: 1.9.1
-	Virtual Size: 16.6 MB (16625930 bytes)
-	v2 Blob: `sha256:6acdef7ebe13fb272b2fb6ac4879f5c815a6e97b34f8f7b46fb3408fddaa03eb`
-	v2 Content-Length: 7.8 MB (7820508 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:26 GMT

#### `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`

```dockerfile
ENV PHP_INI_DIR=/usr/local/etc/php
```

-	Created: Wed, 04 May 2016 03:09:16 GMT
-	Parent Layer: `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`

```dockerfile
RUN mkdir -p $PHP_INI_DIR/conf.d
```

-	Created: Wed, 04 May 2016 03:09:18 GMT
-	Parent Layer: `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:4fc566a7c22ab414ecafcea1db51a7687bfff449c21fcba1ca3ffc8f7431fedc`
-	v2 Content-Length: 180.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:15 GMT

#### `8fd6fb866ea18ab6b5153616e91c4ea9b8b81a3349982b4118bfc347deedfa31`

```dockerfile
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data
```

-	Created: Wed, 04 May 2016 03:25:25 GMT
-	Parent Layer: `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `99f6ec6dca3cae4da6557e122d1acf201ea575cd5f110021d7411509ec0a81d7`

```dockerfile
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
```

-	Created: Wed, 04 May 2016 04:01:20 GMT
-	Parent Layer: `8fd6fb866ea18ab6b5153616e91c4ea9b8b81a3349982b4118bfc347deedfa31`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `40e9019ed184ba8b7b782147cbf8fa32110407807b94ee1d0162298badcd6a9e`

```dockerfile
ENV PHP_VERSION=5.6.21
```

-	Created: Wed, 04 May 2016 04:01:20 GMT
-	Parent Layer: `99f6ec6dca3cae4da6557e122d1acf201ea575cd5f110021d7411509ec0a81d7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `d532422949e5520306554a44dc4a2434ef7902cd8f1d31c5f30c85ca621c82a8`

```dockerfile
ENV PHP_FILENAME=php-5.6.21.tar.xz
```

-	Created: Wed, 04 May 2016 04:01:21 GMT
-	Parent Layer: `40e9019ed184ba8b7b782147cbf8fa32110407807b94ee1d0162298badcd6a9e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `560521cfa49cc2170168481c9890167d13ffb93931368f6da9db34a863288564`

```dockerfile
ENV PHP_SHA256=566ff1a486cb0485ed477a91ea292423f77a58671270ff73b74e67e3ce7084f9
```

-	Created: Wed, 04 May 2016 04:01:22 GMT
-	Parent Layer: `d532422949e5520306554a44dc4a2434ef7902cd8f1d31c5f30c85ca621c82a8`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `520f589892f775eda8a8649dc36fe8c94475094c1b3f7a5a7df404eee49eb55f`

```dockerfile
RUN set -xe \
	&& buildDeps=" \
		$PHP_EXTRA_BUILD_DEPS \
		libcurl4-openssl-dev \
		libedit-dev \
		libsqlite3-dev \
		libssl-dev \
		libxml2-dev \
		xz-utils \
	" \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME/from/this/mirror" -o "$PHP_FILENAME" \
	&& echo "$PHP_SHA256 *$PHP_FILENAME" | sha256sum -c - \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME.asc/from/this/mirror" -o "$PHP_FILENAME.asc" \
	&& export GNUPGHOME="$(mktemp -d)" \
	&& for key in $GPG_KEYS; do \
		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; \
	done \
	&& gpg --batch --verify "$PHP_FILENAME.asc" "$PHP_FILENAME" \
	&& rm -r "$GNUPGHOME" "$PHP_FILENAME.asc" \
	&& mkdir -p /usr/src/php \
	&& tar -xf "$PHP_FILENAME" -C /usr/src/php --strip-components=1 \
	&& rm "$PHP_FILENAME" \
	&& cd /usr/src/php \
	&& ./configure \
		--with-config-file-path="$PHP_INI_DIR" \
		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" \
		$PHP_EXTRA_CONFIGURE_ARGS \
		--disable-cgi \
		--enable-mysqlnd \
		--enable-mbstring \
		--with-curl \
		--with-libedit \
		--with-openssl \
		--with-zlib \
	&& make -j"$(nproc)" \
	&& make install \
	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } \
	&& make clean \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps
```

-	Created: Wed, 04 May 2016 04:07:25 GMT
-	Parent Layer: `560521cfa49cc2170168481c9890167d13ffb93931368f6da9db34a863288564`
-	Docker Version: 1.9.1
-	Virtual Size: 136.3 MB (136300601 bytes)
-	v2 Blob: `sha256:2fa81675c8d53cfe31743f076e9ef9794aa52416ebc7f32a812921355e0ebc66`
-	v2 Content-Length: 26.5 MB (26473544 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:11:34 GMT

#### `efa109fb600faa91854b656c6bcd8b0721f7ce2e908c33dbb78bcf6697a7b87e`

```dockerfile
COPY multi:82b89724359b10e4fa6ed1d5d2d5ab38544995f1ed9288734f40288633831460 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 04:07:30 GMT
-	Parent Layer: `520f589892f775eda8a8649dc36fe8c94475094c1b3f7a5a7df404eee49eb55f`
-	Docker Version: 1.9.1
-	Virtual Size: 3.6 KB (3582 bytes)
-	v2 Blob: `sha256:2b9596305f8a7a19c2103e8bad0ada832f9d4ce0e3a16821c4627f0d0f102026`
-	v2 Content-Length: 1.5 KB (1548 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:11:07 GMT

#### `b29cd7954722ee9db9f0815315dda4487c009fb3d0f3c542fa9b1c274708ca65`

```dockerfile
WORKDIR /var/www/html
```

-	Created: Wed, 04 May 2016 04:07:31 GMT
-	Parent Layer: `efa109fb600faa91854b656c6bcd8b0721f7ce2e908c33dbb78bcf6697a7b87e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `438b852026867eb7dce1c48275da5a1dc4fa4b8809e170a3476dc119e6c1d95b`

```dockerfile
RUN set -ex \
	&& cd /usr/local/etc \
	&& if [ -d php-fpm.d ]; then \
		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; \
		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; \
	else \
		mkdir php-fpm.d; \
		cp php-fpm.conf.default php-fpm.d/www.conf; \
		{ \
			echo '[global]'; \
			echo 'include=etc/php-fpm.d/*.conf'; \
		} | tee php-fpm.conf; \
	fi \
	&& { \
		echo '[global]'; \
		echo 'error_log = /proc/self/fd/2'; \
		echo; \
		echo '[www]'; \
		echo '; if we send this to /proc/self/fd/1, it never appears'; \
		echo 'access.log = /proc/self/fd/2'; \
		echo; \
		echo 'clear_env = no'; \
		echo; \
		echo '; Ensure worker stdout and stderr are sent to the main error log.'; \
		echo 'catch_workers_output = yes'; \
	} | tee php-fpm.d/docker.conf \
	&& { \
		echo '[global]'; \
		echo 'daemonize = no'; \
		echo; \
		echo '[www]'; \
		echo 'listen = [::]:9000'; \
	} | tee php-fpm.d/zz-docker.conf
```

-	Created: Wed, 04 May 2016 04:07:33 GMT
-	Parent Layer: `b29cd7954722ee9db9f0815315dda4487c009fb3d0f3c542fa9b1c274708ca65`
-	Docker Version: 1.9.1
-	Virtual Size: 23.1 KB (23094 bytes)
-	v2 Blob: `sha256:dd763b7ae0fc69ad17ff4bdec9bc4e7dca77de0697e39cbb06d1daff1746f485`
-	v2 Content-Length: 7.7 KB (7683 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:11:01 GMT

#### `a399b1ebfc39b45da6a10012575dddb0ecc8555a83aa3890bcdf21fc62d30d92`

```dockerfile
EXPOSE 9000/tcp
```

-	Created: Wed, 04 May 2016 04:07:33 GMT
-	Parent Layer: `438b852026867eb7dce1c48275da5a1dc4fa4b8809e170a3476dc119e6c1d95b`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `fd19aeb28b3cfa77f4a99088bd64fe84019cec0533037123c7b07442e6957182`

```dockerfile
CMD ["php-fpm"]
```

-	Created: Wed, 04 May 2016 04:07:34 GMT
-	Parent Layer: `a399b1ebfc39b45da6a10012575dddb0ecc8555a83aa3890bcdf21fc62d30d92`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `84e75d5fcd801d02fb39b43bd527ee57d74b623b01fae8606da4a90f23fe9b3f`

```dockerfile
RUN apt-get update && apt-get install -y libpng12-dev libjpeg-dev && rm -rf /var/lib/apt/lists/* \
	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr \
	&& docker-php-ext-install gd mysqli opcache
```

-	Created: Thu, 05 May 2016 06:06:34 GMT
-	Parent Layer: `fd19aeb28b3cfa77f4a99088bd64fe84019cec0533037123c7b07442e6957182`
-	Docker Version: 1.9.1
-	Virtual Size: 14.7 MB (14685145 bytes)
-	v2 Blob: `sha256:0880dc1cc37191527670cff85823ae67dc87cb220d1eeb4a41adb67c163ae302`
-	v2 Content-Length: 4.4 MB (4420999 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 23:38:48 GMT

#### `f639697e9e0ccb63766f00dfb552317abe9664bf82464c116cd890dc037d027e`

```dockerfile
RUN { \
		echo 'opcache.memory_consumption=128'; \
		echo 'opcache.interned_strings_buffer=8'; \
		echo 'opcache.max_accelerated_files=4000'; \
		echo 'opcache.revalidate_freq=60'; \
		echo 'opcache.fast_shutdown=1'; \
		echo 'opcache.enable_cli=1'; \
	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
```

-	Created: Thu, 05 May 2016 06:06:36 GMT
-	Parent Layer: `84e75d5fcd801d02fb39b43bd527ee57d74b623b01fae8606da4a90f23fe9b3f`
-	Docker Version: 1.9.1
-	Virtual Size: 172.0 B
-	v2 Blob: `sha256:cc9ba5c37fd237eb001a3fc70b1d43a8ad4732529b4a19eb8e3cdd00956013cf`
-	v2 Content-Length: 333.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:38:43 GMT

#### `bc1341fe62662a25cf97c82d3d2c6c3e1a1e360fd8ba3b18bce1fc07b81f6da7`

```dockerfile
VOLUME [/var/www/html]
```

-	Created: Thu, 05 May 2016 06:06:37 GMT
-	Parent Layer: `f639697e9e0ccb63766f00dfb552317abe9664bf82464c116cd890dc037d027e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `3508ddf1c8913c5591dc5ca7361006d3adfb4c4278346293a07d868efc3fb871`

```dockerfile
ENV WORDPRESS_VERSION=4.5.2
```

-	Created: Tue, 10 May 2016 01:29:57 GMT
-	Parent Layer: `bc1341fe62662a25cf97c82d3d2c6c3e1a1e360fd8ba3b18bce1fc07b81f6da7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `9a38934c092657f835f3042b4f56c8bca813f2b991d9fff26b8f8e9147aa07ca`

```dockerfile
ENV WORDPRESS_SHA1=bab94003a5d2285f6ae76407e7b1bbb75382c36e
```

-	Created: Tue, 10 May 2016 01:29:57 GMT
-	Parent Layer: `3508ddf1c8913c5591dc5ca7361006d3adfb4c4278346293a07d868efc3fb871`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `b72c4991df3200068f40a98e47d1ff0e9f5c94170c3c3a71012bef1603fcb994`

```dockerfile
RUN curl -o wordpress.tar.gz -SL https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz \
	&& echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c - \
	&& tar -xzf wordpress.tar.gz -C /usr/src/ \
	&& rm wordpress.tar.gz \
	&& chown -R www-data:www-data /usr/src/wordpress
```

-	Created: Tue, 10 May 2016 01:29:59 GMT
-	Parent Layer: `9a38934c092657f835f3042b4f56c8bca813f2b991d9fff26b8f8e9147aa07ca`
-	Docker Version: 1.9.1
-	Virtual Size: 21.9 MB (21908610 bytes)
-	v2 Blob: `sha256:817016e1ab05a17b14fc1abea031b00439450cd6f47e68cf84032582aa92bcef`
-	v2 Content-Length: 7.6 MB (7610170 bytes)
-	v2 Last-Modified: Tue, 10 May 2016 01:56:47 GMT

#### `1b78f1bff6be5744b7ed32aa5e86f3bbe0c743bfea2e7cb7b33d88c272694002`

```dockerfile
COPY file:e4f27140dddd16cd34ce106cb7587b487bdf49693a3436dc23a89fcb0f933d05 in /entrypoint.sh
```

-	Created: Thu, 12 May 2016 19:24:58 GMT
-	Parent Layer: `b72c4991df3200068f40a98e47d1ff0e9f5c94170c3c3a71012bef1603fcb994`
-	Docker Version: 1.9.1
-	Virtual Size: 5.2 KB (5155 bytes)
-	v2 Blob: `sha256:f79a39a56bc213acb9b5131bb94562383aecb31e2c72086fafd6aa36a9617201`
-	v2 Content-Length: 2.5 KB (2492 bytes)
-	v2 Last-Modified: Thu, 12 May 2016 20:00:20 GMT

#### `a2e083a2d07a138c1f313a0f22155f1a2c8734dca13c643a7a9ae543bc7b6295`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Thu, 12 May 2016 19:24:58 GMT
-	Parent Layer: `1b78f1bff6be5744b7ed32aa5e86f3bbe0c743bfea2e7cb7b33d88c272694002`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `fa2fb79917c7b14115b62924f251fdc3cca863b981948cf9b95214f74f11ad07`

```dockerfile
CMD ["php-fpm"]
```

-	Created: Thu, 12 May 2016 19:24:59 GMT
-	Parent Layer: `a2e083a2d07a138c1f313a0f22155f1a2c8734dca13c643a7a9ae543bc7b6295`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

## `wordpress:4.5-fpm`

```console
$ docker pull library/wordpress@sha256:7da1d0384853970b2162267136b698a996c4922ff7994caeb70bfcf1faa0e54d
```

-	Total Virtual Size: 492.4 MB (492434366 bytes)
-	Total v2 Content-Length: 167.3 MB (167260138 bytes)

### Layers (26)

#### `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`

```dockerfile
ADD file:dc2eddd5d35b9d66e4db747f5939b2be7f863dcee64c934b0da690f55a23aee8 in /
```

-	Created: Tue, 03 May 2016 20:57:39 GMT
-	Docker Version: 1.9.1
-	Virtual Size: 125.1 MB (125093399 bytes)
-	v2 Blob: `sha256:8b87079b7a06f9b72e3cca2c984c60e118229c60f0bff855d822f758c112b485`
-	v2 Content-Length: 51.4 MB (51355855 bytes)
-	v2 Last-Modified: Tue, 03 May 2016 20:59:55 GMT

#### `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Tue, 03 May 2016 20:57:42 GMT
-	Parent Layer: `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`

```dockerfile
RUN apt-get update && apt-get install -y \
		autoconf \
		file \
		g++ \
		gcc \
		libc-dev \
		make \
		pkg-config \
		re2c \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:08:29 GMT
-	Parent Layer: `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`
-	Docker Version: 1.9.1
-	Virtual Size: 177.8 MB (177788678 bytes)
-	v2 Blob: `sha256:af1704cb90e1fa3243238682e49412335aba819dc71452142be0a48851ba039a`
-	v2 Content-Length: 69.6 MB (69566346 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:08:02 GMT

#### `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`

```dockerfile
RUN apt-get update && apt-get install -y \
		ca-certificates \
		curl \
		libedit2 \
		libsqlite3-0 \
		libxml2 \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:09:15 GMT
-	Parent Layer: `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`
-	Docker Version: 1.9.1
-	Virtual Size: 16.6 MB (16625930 bytes)
-	v2 Blob: `sha256:6acdef7ebe13fb272b2fb6ac4879f5c815a6e97b34f8f7b46fb3408fddaa03eb`
-	v2 Content-Length: 7.8 MB (7820508 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:26 GMT

#### `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`

```dockerfile
ENV PHP_INI_DIR=/usr/local/etc/php
```

-	Created: Wed, 04 May 2016 03:09:16 GMT
-	Parent Layer: `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`

```dockerfile
RUN mkdir -p $PHP_INI_DIR/conf.d
```

-	Created: Wed, 04 May 2016 03:09:18 GMT
-	Parent Layer: `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:4fc566a7c22ab414ecafcea1db51a7687bfff449c21fcba1ca3ffc8f7431fedc`
-	v2 Content-Length: 180.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:15 GMT

#### `8fd6fb866ea18ab6b5153616e91c4ea9b8b81a3349982b4118bfc347deedfa31`

```dockerfile
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data
```

-	Created: Wed, 04 May 2016 03:25:25 GMT
-	Parent Layer: `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `99f6ec6dca3cae4da6557e122d1acf201ea575cd5f110021d7411509ec0a81d7`

```dockerfile
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
```

-	Created: Wed, 04 May 2016 04:01:20 GMT
-	Parent Layer: `8fd6fb866ea18ab6b5153616e91c4ea9b8b81a3349982b4118bfc347deedfa31`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `40e9019ed184ba8b7b782147cbf8fa32110407807b94ee1d0162298badcd6a9e`

```dockerfile
ENV PHP_VERSION=5.6.21
```

-	Created: Wed, 04 May 2016 04:01:20 GMT
-	Parent Layer: `99f6ec6dca3cae4da6557e122d1acf201ea575cd5f110021d7411509ec0a81d7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `d532422949e5520306554a44dc4a2434ef7902cd8f1d31c5f30c85ca621c82a8`

```dockerfile
ENV PHP_FILENAME=php-5.6.21.tar.xz
```

-	Created: Wed, 04 May 2016 04:01:21 GMT
-	Parent Layer: `40e9019ed184ba8b7b782147cbf8fa32110407807b94ee1d0162298badcd6a9e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `560521cfa49cc2170168481c9890167d13ffb93931368f6da9db34a863288564`

```dockerfile
ENV PHP_SHA256=566ff1a486cb0485ed477a91ea292423f77a58671270ff73b74e67e3ce7084f9
```

-	Created: Wed, 04 May 2016 04:01:22 GMT
-	Parent Layer: `d532422949e5520306554a44dc4a2434ef7902cd8f1d31c5f30c85ca621c82a8`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `520f589892f775eda8a8649dc36fe8c94475094c1b3f7a5a7df404eee49eb55f`

```dockerfile
RUN set -xe \
	&& buildDeps=" \
		$PHP_EXTRA_BUILD_DEPS \
		libcurl4-openssl-dev \
		libedit-dev \
		libsqlite3-dev \
		libssl-dev \
		libxml2-dev \
		xz-utils \
	" \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME/from/this/mirror" -o "$PHP_FILENAME" \
	&& echo "$PHP_SHA256 *$PHP_FILENAME" | sha256sum -c - \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME.asc/from/this/mirror" -o "$PHP_FILENAME.asc" \
	&& export GNUPGHOME="$(mktemp -d)" \
	&& for key in $GPG_KEYS; do \
		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; \
	done \
	&& gpg --batch --verify "$PHP_FILENAME.asc" "$PHP_FILENAME" \
	&& rm -r "$GNUPGHOME" "$PHP_FILENAME.asc" \
	&& mkdir -p /usr/src/php \
	&& tar -xf "$PHP_FILENAME" -C /usr/src/php --strip-components=1 \
	&& rm "$PHP_FILENAME" \
	&& cd /usr/src/php \
	&& ./configure \
		--with-config-file-path="$PHP_INI_DIR" \
		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" \
		$PHP_EXTRA_CONFIGURE_ARGS \
		--disable-cgi \
		--enable-mysqlnd \
		--enable-mbstring \
		--with-curl \
		--with-libedit \
		--with-openssl \
		--with-zlib \
	&& make -j"$(nproc)" \
	&& make install \
	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } \
	&& make clean \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps
```

-	Created: Wed, 04 May 2016 04:07:25 GMT
-	Parent Layer: `560521cfa49cc2170168481c9890167d13ffb93931368f6da9db34a863288564`
-	Docker Version: 1.9.1
-	Virtual Size: 136.3 MB (136300601 bytes)
-	v2 Blob: `sha256:2fa81675c8d53cfe31743f076e9ef9794aa52416ebc7f32a812921355e0ebc66`
-	v2 Content-Length: 26.5 MB (26473544 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:11:34 GMT

#### `efa109fb600faa91854b656c6bcd8b0721f7ce2e908c33dbb78bcf6697a7b87e`

```dockerfile
COPY multi:82b89724359b10e4fa6ed1d5d2d5ab38544995f1ed9288734f40288633831460 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 04:07:30 GMT
-	Parent Layer: `520f589892f775eda8a8649dc36fe8c94475094c1b3f7a5a7df404eee49eb55f`
-	Docker Version: 1.9.1
-	Virtual Size: 3.6 KB (3582 bytes)
-	v2 Blob: `sha256:2b9596305f8a7a19c2103e8bad0ada832f9d4ce0e3a16821c4627f0d0f102026`
-	v2 Content-Length: 1.5 KB (1548 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:11:07 GMT

#### `b29cd7954722ee9db9f0815315dda4487c009fb3d0f3c542fa9b1c274708ca65`

```dockerfile
WORKDIR /var/www/html
```

-	Created: Wed, 04 May 2016 04:07:31 GMT
-	Parent Layer: `efa109fb600faa91854b656c6bcd8b0721f7ce2e908c33dbb78bcf6697a7b87e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `438b852026867eb7dce1c48275da5a1dc4fa4b8809e170a3476dc119e6c1d95b`

```dockerfile
RUN set -ex \
	&& cd /usr/local/etc \
	&& if [ -d php-fpm.d ]; then \
		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; \
		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; \
	else \
		mkdir php-fpm.d; \
		cp php-fpm.conf.default php-fpm.d/www.conf; \
		{ \
			echo '[global]'; \
			echo 'include=etc/php-fpm.d/*.conf'; \
		} | tee php-fpm.conf; \
	fi \
	&& { \
		echo '[global]'; \
		echo 'error_log = /proc/self/fd/2'; \
		echo; \
		echo '[www]'; \
		echo '; if we send this to /proc/self/fd/1, it never appears'; \
		echo 'access.log = /proc/self/fd/2'; \
		echo; \
		echo 'clear_env = no'; \
		echo; \
		echo '; Ensure worker stdout and stderr are sent to the main error log.'; \
		echo 'catch_workers_output = yes'; \
	} | tee php-fpm.d/docker.conf \
	&& { \
		echo '[global]'; \
		echo 'daemonize = no'; \
		echo; \
		echo '[www]'; \
		echo 'listen = [::]:9000'; \
	} | tee php-fpm.d/zz-docker.conf
```

-	Created: Wed, 04 May 2016 04:07:33 GMT
-	Parent Layer: `b29cd7954722ee9db9f0815315dda4487c009fb3d0f3c542fa9b1c274708ca65`
-	Docker Version: 1.9.1
-	Virtual Size: 23.1 KB (23094 bytes)
-	v2 Blob: `sha256:dd763b7ae0fc69ad17ff4bdec9bc4e7dca77de0697e39cbb06d1daff1746f485`
-	v2 Content-Length: 7.7 KB (7683 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:11:01 GMT

#### `a399b1ebfc39b45da6a10012575dddb0ecc8555a83aa3890bcdf21fc62d30d92`

```dockerfile
EXPOSE 9000/tcp
```

-	Created: Wed, 04 May 2016 04:07:33 GMT
-	Parent Layer: `438b852026867eb7dce1c48275da5a1dc4fa4b8809e170a3476dc119e6c1d95b`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `fd19aeb28b3cfa77f4a99088bd64fe84019cec0533037123c7b07442e6957182`

```dockerfile
CMD ["php-fpm"]
```

-	Created: Wed, 04 May 2016 04:07:34 GMT
-	Parent Layer: `a399b1ebfc39b45da6a10012575dddb0ecc8555a83aa3890bcdf21fc62d30d92`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `84e75d5fcd801d02fb39b43bd527ee57d74b623b01fae8606da4a90f23fe9b3f`

```dockerfile
RUN apt-get update && apt-get install -y libpng12-dev libjpeg-dev && rm -rf /var/lib/apt/lists/* \
	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr \
	&& docker-php-ext-install gd mysqli opcache
```

-	Created: Thu, 05 May 2016 06:06:34 GMT
-	Parent Layer: `fd19aeb28b3cfa77f4a99088bd64fe84019cec0533037123c7b07442e6957182`
-	Docker Version: 1.9.1
-	Virtual Size: 14.7 MB (14685145 bytes)
-	v2 Blob: `sha256:0880dc1cc37191527670cff85823ae67dc87cb220d1eeb4a41adb67c163ae302`
-	v2 Content-Length: 4.4 MB (4420999 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 23:38:48 GMT

#### `f639697e9e0ccb63766f00dfb552317abe9664bf82464c116cd890dc037d027e`

```dockerfile
RUN { \
		echo 'opcache.memory_consumption=128'; \
		echo 'opcache.interned_strings_buffer=8'; \
		echo 'opcache.max_accelerated_files=4000'; \
		echo 'opcache.revalidate_freq=60'; \
		echo 'opcache.fast_shutdown=1'; \
		echo 'opcache.enable_cli=1'; \
	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
```

-	Created: Thu, 05 May 2016 06:06:36 GMT
-	Parent Layer: `84e75d5fcd801d02fb39b43bd527ee57d74b623b01fae8606da4a90f23fe9b3f`
-	Docker Version: 1.9.1
-	Virtual Size: 172.0 B
-	v2 Blob: `sha256:cc9ba5c37fd237eb001a3fc70b1d43a8ad4732529b4a19eb8e3cdd00956013cf`
-	v2 Content-Length: 333.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:38:43 GMT

#### `bc1341fe62662a25cf97c82d3d2c6c3e1a1e360fd8ba3b18bce1fc07b81f6da7`

```dockerfile
VOLUME [/var/www/html]
```

-	Created: Thu, 05 May 2016 06:06:37 GMT
-	Parent Layer: `f639697e9e0ccb63766f00dfb552317abe9664bf82464c116cd890dc037d027e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `3508ddf1c8913c5591dc5ca7361006d3adfb4c4278346293a07d868efc3fb871`

```dockerfile
ENV WORDPRESS_VERSION=4.5.2
```

-	Created: Tue, 10 May 2016 01:29:57 GMT
-	Parent Layer: `bc1341fe62662a25cf97c82d3d2c6c3e1a1e360fd8ba3b18bce1fc07b81f6da7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `9a38934c092657f835f3042b4f56c8bca813f2b991d9fff26b8f8e9147aa07ca`

```dockerfile
ENV WORDPRESS_SHA1=bab94003a5d2285f6ae76407e7b1bbb75382c36e
```

-	Created: Tue, 10 May 2016 01:29:57 GMT
-	Parent Layer: `3508ddf1c8913c5591dc5ca7361006d3adfb4c4278346293a07d868efc3fb871`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `b72c4991df3200068f40a98e47d1ff0e9f5c94170c3c3a71012bef1603fcb994`

```dockerfile
RUN curl -o wordpress.tar.gz -SL https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz \
	&& echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c - \
	&& tar -xzf wordpress.tar.gz -C /usr/src/ \
	&& rm wordpress.tar.gz \
	&& chown -R www-data:www-data /usr/src/wordpress
```

-	Created: Tue, 10 May 2016 01:29:59 GMT
-	Parent Layer: `9a38934c092657f835f3042b4f56c8bca813f2b991d9fff26b8f8e9147aa07ca`
-	Docker Version: 1.9.1
-	Virtual Size: 21.9 MB (21908610 bytes)
-	v2 Blob: `sha256:817016e1ab05a17b14fc1abea031b00439450cd6f47e68cf84032582aa92bcef`
-	v2 Content-Length: 7.6 MB (7610170 bytes)
-	v2 Last-Modified: Tue, 10 May 2016 01:56:47 GMT

#### `1b78f1bff6be5744b7ed32aa5e86f3bbe0c743bfea2e7cb7b33d88c272694002`

```dockerfile
COPY file:e4f27140dddd16cd34ce106cb7587b487bdf49693a3436dc23a89fcb0f933d05 in /entrypoint.sh
```

-	Created: Thu, 12 May 2016 19:24:58 GMT
-	Parent Layer: `b72c4991df3200068f40a98e47d1ff0e9f5c94170c3c3a71012bef1603fcb994`
-	Docker Version: 1.9.1
-	Virtual Size: 5.2 KB (5155 bytes)
-	v2 Blob: `sha256:f79a39a56bc213acb9b5131bb94562383aecb31e2c72086fafd6aa36a9617201`
-	v2 Content-Length: 2.5 KB (2492 bytes)
-	v2 Last-Modified: Thu, 12 May 2016 20:00:20 GMT

#### `a2e083a2d07a138c1f313a0f22155f1a2c8734dca13c643a7a9ae543bc7b6295`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Thu, 12 May 2016 19:24:58 GMT
-	Parent Layer: `1b78f1bff6be5744b7ed32aa5e86f3bbe0c743bfea2e7cb7b33d88c272694002`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `fa2fb79917c7b14115b62924f251fdc3cca863b981948cf9b95214f74f11ad07`

```dockerfile
CMD ["php-fpm"]
```

-	Created: Thu, 12 May 2016 19:24:59 GMT
-	Parent Layer: `a2e083a2d07a138c1f313a0f22155f1a2c8734dca13c643a7a9ae543bc7b6295`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

## `wordpress:4-fpm`

```console
$ docker pull library/wordpress@sha256:6c19f08a8fabf815e545fd485ac10bc83644598d84fdf34c4c91057afd410c5a
```

-	Total Virtual Size: 492.4 MB (492434366 bytes)
-	Total v2 Content-Length: 167.3 MB (167260138 bytes)

### Layers (26)

#### `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`

```dockerfile
ADD file:dc2eddd5d35b9d66e4db747f5939b2be7f863dcee64c934b0da690f55a23aee8 in /
```

-	Created: Tue, 03 May 2016 20:57:39 GMT
-	Docker Version: 1.9.1
-	Virtual Size: 125.1 MB (125093399 bytes)
-	v2 Blob: `sha256:8b87079b7a06f9b72e3cca2c984c60e118229c60f0bff855d822f758c112b485`
-	v2 Content-Length: 51.4 MB (51355855 bytes)
-	v2 Last-Modified: Tue, 03 May 2016 20:59:55 GMT

#### `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Tue, 03 May 2016 20:57:42 GMT
-	Parent Layer: `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`

```dockerfile
RUN apt-get update && apt-get install -y \
		autoconf \
		file \
		g++ \
		gcc \
		libc-dev \
		make \
		pkg-config \
		re2c \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:08:29 GMT
-	Parent Layer: `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`
-	Docker Version: 1.9.1
-	Virtual Size: 177.8 MB (177788678 bytes)
-	v2 Blob: `sha256:af1704cb90e1fa3243238682e49412335aba819dc71452142be0a48851ba039a`
-	v2 Content-Length: 69.6 MB (69566346 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:08:02 GMT

#### `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`

```dockerfile
RUN apt-get update && apt-get install -y \
		ca-certificates \
		curl \
		libedit2 \
		libsqlite3-0 \
		libxml2 \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:09:15 GMT
-	Parent Layer: `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`
-	Docker Version: 1.9.1
-	Virtual Size: 16.6 MB (16625930 bytes)
-	v2 Blob: `sha256:6acdef7ebe13fb272b2fb6ac4879f5c815a6e97b34f8f7b46fb3408fddaa03eb`
-	v2 Content-Length: 7.8 MB (7820508 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:26 GMT

#### `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`

```dockerfile
ENV PHP_INI_DIR=/usr/local/etc/php
```

-	Created: Wed, 04 May 2016 03:09:16 GMT
-	Parent Layer: `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`

```dockerfile
RUN mkdir -p $PHP_INI_DIR/conf.d
```

-	Created: Wed, 04 May 2016 03:09:18 GMT
-	Parent Layer: `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:4fc566a7c22ab414ecafcea1db51a7687bfff449c21fcba1ca3ffc8f7431fedc`
-	v2 Content-Length: 180.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:15 GMT

#### `8fd6fb866ea18ab6b5153616e91c4ea9b8b81a3349982b4118bfc347deedfa31`

```dockerfile
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data
```

-	Created: Wed, 04 May 2016 03:25:25 GMT
-	Parent Layer: `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `99f6ec6dca3cae4da6557e122d1acf201ea575cd5f110021d7411509ec0a81d7`

```dockerfile
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
```

-	Created: Wed, 04 May 2016 04:01:20 GMT
-	Parent Layer: `8fd6fb866ea18ab6b5153616e91c4ea9b8b81a3349982b4118bfc347deedfa31`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `40e9019ed184ba8b7b782147cbf8fa32110407807b94ee1d0162298badcd6a9e`

```dockerfile
ENV PHP_VERSION=5.6.21
```

-	Created: Wed, 04 May 2016 04:01:20 GMT
-	Parent Layer: `99f6ec6dca3cae4da6557e122d1acf201ea575cd5f110021d7411509ec0a81d7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `d532422949e5520306554a44dc4a2434ef7902cd8f1d31c5f30c85ca621c82a8`

```dockerfile
ENV PHP_FILENAME=php-5.6.21.tar.xz
```

-	Created: Wed, 04 May 2016 04:01:21 GMT
-	Parent Layer: `40e9019ed184ba8b7b782147cbf8fa32110407807b94ee1d0162298badcd6a9e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `560521cfa49cc2170168481c9890167d13ffb93931368f6da9db34a863288564`

```dockerfile
ENV PHP_SHA256=566ff1a486cb0485ed477a91ea292423f77a58671270ff73b74e67e3ce7084f9
```

-	Created: Wed, 04 May 2016 04:01:22 GMT
-	Parent Layer: `d532422949e5520306554a44dc4a2434ef7902cd8f1d31c5f30c85ca621c82a8`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `520f589892f775eda8a8649dc36fe8c94475094c1b3f7a5a7df404eee49eb55f`

```dockerfile
RUN set -xe \
	&& buildDeps=" \
		$PHP_EXTRA_BUILD_DEPS \
		libcurl4-openssl-dev \
		libedit-dev \
		libsqlite3-dev \
		libssl-dev \
		libxml2-dev \
		xz-utils \
	" \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME/from/this/mirror" -o "$PHP_FILENAME" \
	&& echo "$PHP_SHA256 *$PHP_FILENAME" | sha256sum -c - \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME.asc/from/this/mirror" -o "$PHP_FILENAME.asc" \
	&& export GNUPGHOME="$(mktemp -d)" \
	&& for key in $GPG_KEYS; do \
		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; \
	done \
	&& gpg --batch --verify "$PHP_FILENAME.asc" "$PHP_FILENAME" \
	&& rm -r "$GNUPGHOME" "$PHP_FILENAME.asc" \
	&& mkdir -p /usr/src/php \
	&& tar -xf "$PHP_FILENAME" -C /usr/src/php --strip-components=1 \
	&& rm "$PHP_FILENAME" \
	&& cd /usr/src/php \
	&& ./configure \
		--with-config-file-path="$PHP_INI_DIR" \
		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" \
		$PHP_EXTRA_CONFIGURE_ARGS \
		--disable-cgi \
		--enable-mysqlnd \
		--enable-mbstring \
		--with-curl \
		--with-libedit \
		--with-openssl \
		--with-zlib \
	&& make -j"$(nproc)" \
	&& make install \
	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } \
	&& make clean \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps
```

-	Created: Wed, 04 May 2016 04:07:25 GMT
-	Parent Layer: `560521cfa49cc2170168481c9890167d13ffb93931368f6da9db34a863288564`
-	Docker Version: 1.9.1
-	Virtual Size: 136.3 MB (136300601 bytes)
-	v2 Blob: `sha256:2fa81675c8d53cfe31743f076e9ef9794aa52416ebc7f32a812921355e0ebc66`
-	v2 Content-Length: 26.5 MB (26473544 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:11:34 GMT

#### `efa109fb600faa91854b656c6bcd8b0721f7ce2e908c33dbb78bcf6697a7b87e`

```dockerfile
COPY multi:82b89724359b10e4fa6ed1d5d2d5ab38544995f1ed9288734f40288633831460 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 04:07:30 GMT
-	Parent Layer: `520f589892f775eda8a8649dc36fe8c94475094c1b3f7a5a7df404eee49eb55f`
-	Docker Version: 1.9.1
-	Virtual Size: 3.6 KB (3582 bytes)
-	v2 Blob: `sha256:2b9596305f8a7a19c2103e8bad0ada832f9d4ce0e3a16821c4627f0d0f102026`
-	v2 Content-Length: 1.5 KB (1548 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:11:07 GMT

#### `b29cd7954722ee9db9f0815315dda4487c009fb3d0f3c542fa9b1c274708ca65`

```dockerfile
WORKDIR /var/www/html
```

-	Created: Wed, 04 May 2016 04:07:31 GMT
-	Parent Layer: `efa109fb600faa91854b656c6bcd8b0721f7ce2e908c33dbb78bcf6697a7b87e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `438b852026867eb7dce1c48275da5a1dc4fa4b8809e170a3476dc119e6c1d95b`

```dockerfile
RUN set -ex \
	&& cd /usr/local/etc \
	&& if [ -d php-fpm.d ]; then \
		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; \
		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; \
	else \
		mkdir php-fpm.d; \
		cp php-fpm.conf.default php-fpm.d/www.conf; \
		{ \
			echo '[global]'; \
			echo 'include=etc/php-fpm.d/*.conf'; \
		} | tee php-fpm.conf; \
	fi \
	&& { \
		echo '[global]'; \
		echo 'error_log = /proc/self/fd/2'; \
		echo; \
		echo '[www]'; \
		echo '; if we send this to /proc/self/fd/1, it never appears'; \
		echo 'access.log = /proc/self/fd/2'; \
		echo; \
		echo 'clear_env = no'; \
		echo; \
		echo '; Ensure worker stdout and stderr are sent to the main error log.'; \
		echo 'catch_workers_output = yes'; \
	} | tee php-fpm.d/docker.conf \
	&& { \
		echo '[global]'; \
		echo 'daemonize = no'; \
		echo; \
		echo '[www]'; \
		echo 'listen = [::]:9000'; \
	} | tee php-fpm.d/zz-docker.conf
```

-	Created: Wed, 04 May 2016 04:07:33 GMT
-	Parent Layer: `b29cd7954722ee9db9f0815315dda4487c009fb3d0f3c542fa9b1c274708ca65`
-	Docker Version: 1.9.1
-	Virtual Size: 23.1 KB (23094 bytes)
-	v2 Blob: `sha256:dd763b7ae0fc69ad17ff4bdec9bc4e7dca77de0697e39cbb06d1daff1746f485`
-	v2 Content-Length: 7.7 KB (7683 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:11:01 GMT

#### `a399b1ebfc39b45da6a10012575dddb0ecc8555a83aa3890bcdf21fc62d30d92`

```dockerfile
EXPOSE 9000/tcp
```

-	Created: Wed, 04 May 2016 04:07:33 GMT
-	Parent Layer: `438b852026867eb7dce1c48275da5a1dc4fa4b8809e170a3476dc119e6c1d95b`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `fd19aeb28b3cfa77f4a99088bd64fe84019cec0533037123c7b07442e6957182`

```dockerfile
CMD ["php-fpm"]
```

-	Created: Wed, 04 May 2016 04:07:34 GMT
-	Parent Layer: `a399b1ebfc39b45da6a10012575dddb0ecc8555a83aa3890bcdf21fc62d30d92`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `84e75d5fcd801d02fb39b43bd527ee57d74b623b01fae8606da4a90f23fe9b3f`

```dockerfile
RUN apt-get update && apt-get install -y libpng12-dev libjpeg-dev && rm -rf /var/lib/apt/lists/* \
	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr \
	&& docker-php-ext-install gd mysqli opcache
```

-	Created: Thu, 05 May 2016 06:06:34 GMT
-	Parent Layer: `fd19aeb28b3cfa77f4a99088bd64fe84019cec0533037123c7b07442e6957182`
-	Docker Version: 1.9.1
-	Virtual Size: 14.7 MB (14685145 bytes)
-	v2 Blob: `sha256:0880dc1cc37191527670cff85823ae67dc87cb220d1eeb4a41adb67c163ae302`
-	v2 Content-Length: 4.4 MB (4420999 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 23:38:48 GMT

#### `f639697e9e0ccb63766f00dfb552317abe9664bf82464c116cd890dc037d027e`

```dockerfile
RUN { \
		echo 'opcache.memory_consumption=128'; \
		echo 'opcache.interned_strings_buffer=8'; \
		echo 'opcache.max_accelerated_files=4000'; \
		echo 'opcache.revalidate_freq=60'; \
		echo 'opcache.fast_shutdown=1'; \
		echo 'opcache.enable_cli=1'; \
	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
```

-	Created: Thu, 05 May 2016 06:06:36 GMT
-	Parent Layer: `84e75d5fcd801d02fb39b43bd527ee57d74b623b01fae8606da4a90f23fe9b3f`
-	Docker Version: 1.9.1
-	Virtual Size: 172.0 B
-	v2 Blob: `sha256:cc9ba5c37fd237eb001a3fc70b1d43a8ad4732529b4a19eb8e3cdd00956013cf`
-	v2 Content-Length: 333.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:38:43 GMT

#### `bc1341fe62662a25cf97c82d3d2c6c3e1a1e360fd8ba3b18bce1fc07b81f6da7`

```dockerfile
VOLUME [/var/www/html]
```

-	Created: Thu, 05 May 2016 06:06:37 GMT
-	Parent Layer: `f639697e9e0ccb63766f00dfb552317abe9664bf82464c116cd890dc037d027e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `3508ddf1c8913c5591dc5ca7361006d3adfb4c4278346293a07d868efc3fb871`

```dockerfile
ENV WORDPRESS_VERSION=4.5.2
```

-	Created: Tue, 10 May 2016 01:29:57 GMT
-	Parent Layer: `bc1341fe62662a25cf97c82d3d2c6c3e1a1e360fd8ba3b18bce1fc07b81f6da7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `9a38934c092657f835f3042b4f56c8bca813f2b991d9fff26b8f8e9147aa07ca`

```dockerfile
ENV WORDPRESS_SHA1=bab94003a5d2285f6ae76407e7b1bbb75382c36e
```

-	Created: Tue, 10 May 2016 01:29:57 GMT
-	Parent Layer: `3508ddf1c8913c5591dc5ca7361006d3adfb4c4278346293a07d868efc3fb871`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `b72c4991df3200068f40a98e47d1ff0e9f5c94170c3c3a71012bef1603fcb994`

```dockerfile
RUN curl -o wordpress.tar.gz -SL https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz \
	&& echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c - \
	&& tar -xzf wordpress.tar.gz -C /usr/src/ \
	&& rm wordpress.tar.gz \
	&& chown -R www-data:www-data /usr/src/wordpress
```

-	Created: Tue, 10 May 2016 01:29:59 GMT
-	Parent Layer: `9a38934c092657f835f3042b4f56c8bca813f2b991d9fff26b8f8e9147aa07ca`
-	Docker Version: 1.9.1
-	Virtual Size: 21.9 MB (21908610 bytes)
-	v2 Blob: `sha256:817016e1ab05a17b14fc1abea031b00439450cd6f47e68cf84032582aa92bcef`
-	v2 Content-Length: 7.6 MB (7610170 bytes)
-	v2 Last-Modified: Tue, 10 May 2016 01:56:47 GMT

#### `1b78f1bff6be5744b7ed32aa5e86f3bbe0c743bfea2e7cb7b33d88c272694002`

```dockerfile
COPY file:e4f27140dddd16cd34ce106cb7587b487bdf49693a3436dc23a89fcb0f933d05 in /entrypoint.sh
```

-	Created: Thu, 12 May 2016 19:24:58 GMT
-	Parent Layer: `b72c4991df3200068f40a98e47d1ff0e9f5c94170c3c3a71012bef1603fcb994`
-	Docker Version: 1.9.1
-	Virtual Size: 5.2 KB (5155 bytes)
-	v2 Blob: `sha256:f79a39a56bc213acb9b5131bb94562383aecb31e2c72086fafd6aa36a9617201`
-	v2 Content-Length: 2.5 KB (2492 bytes)
-	v2 Last-Modified: Thu, 12 May 2016 20:00:20 GMT

#### `a2e083a2d07a138c1f313a0f22155f1a2c8734dca13c643a7a9ae543bc7b6295`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Thu, 12 May 2016 19:24:58 GMT
-	Parent Layer: `1b78f1bff6be5744b7ed32aa5e86f3bbe0c743bfea2e7cb7b33d88c272694002`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `fa2fb79917c7b14115b62924f251fdc3cca863b981948cf9b95214f74f11ad07`

```dockerfile
CMD ["php-fpm"]
```

-	Created: Thu, 12 May 2016 19:24:59 GMT
-	Parent Layer: `a2e083a2d07a138c1f313a0f22155f1a2c8734dca13c643a7a9ae543bc7b6295`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

## `wordpress:fpm`

```console
$ docker pull library/wordpress@sha256:3ff233ad14cee0ccdd8ce77bea56231c33bb1b00d928644ce7a2fd51dde32b17
```

-	Total Virtual Size: 492.4 MB (492434366 bytes)
-	Total v2 Content-Length: 167.3 MB (167260138 bytes)

### Layers (26)

#### `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`

```dockerfile
ADD file:dc2eddd5d35b9d66e4db747f5939b2be7f863dcee64c934b0da690f55a23aee8 in /
```

-	Created: Tue, 03 May 2016 20:57:39 GMT
-	Docker Version: 1.9.1
-	Virtual Size: 125.1 MB (125093399 bytes)
-	v2 Blob: `sha256:8b87079b7a06f9b72e3cca2c984c60e118229c60f0bff855d822f758c112b485`
-	v2 Content-Length: 51.4 MB (51355855 bytes)
-	v2 Last-Modified: Tue, 03 May 2016 20:59:55 GMT

#### `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`

```dockerfile
CMD ["/bin/bash"]
```

-	Created: Tue, 03 May 2016 20:57:42 GMT
-	Parent Layer: `e9fa146e2b2b375fd4c6b096b63eff61065f6cbe15b8606932f838bfb708b8cb`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`

```dockerfile
RUN apt-get update && apt-get install -y \
		autoconf \
		file \
		g++ \
		gcc \
		libc-dev \
		make \
		pkg-config \
		re2c \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:08:29 GMT
-	Parent Layer: `ebdf1cd8a5745e8a97e9806392cdd69469620bff2e3ee5a7bd51a5a1f4300904`
-	Docker Version: 1.9.1
-	Virtual Size: 177.8 MB (177788678 bytes)
-	v2 Blob: `sha256:af1704cb90e1fa3243238682e49412335aba819dc71452142be0a48851ba039a`
-	v2 Content-Length: 69.6 MB (69566346 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:08:02 GMT

#### `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`

```dockerfile
RUN apt-get update && apt-get install -y \
		ca-certificates \
		curl \
		libedit2 \
		libsqlite3-0 \
		libxml2 \
	--no-install-recommends && rm -r /var/lib/apt/lists/*
```

-	Created: Wed, 04 May 2016 03:09:15 GMT
-	Parent Layer: `e1703e14b05f1558063730c6fd39f685b14b3ca0759260391edc264ef50f1853`
-	Docker Version: 1.9.1
-	Virtual Size: 16.6 MB (16625930 bytes)
-	v2 Blob: `sha256:6acdef7ebe13fb272b2fb6ac4879f5c815a6e97b34f8f7b46fb3408fddaa03eb`
-	v2 Content-Length: 7.8 MB (7820508 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:07:26 GMT

#### `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`

```dockerfile
ENV PHP_INI_DIR=/usr/local/etc/php
```

-	Created: Wed, 04 May 2016 03:09:16 GMT
-	Parent Layer: `95131299c7218840d87b0ec7a831517280a6846d7309c86f2b994928999ac078`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`

```dockerfile
RUN mkdir -p $PHP_INI_DIR/conf.d
```

-	Created: Wed, 04 May 2016 03:09:18 GMT
-	Parent Layer: `df42d09f67769f95b2a775e3f4fa330dc6028791a313dc76485e5e5bef2cb7b4`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:4fc566a7c22ab414ecafcea1db51a7687bfff449c21fcba1ca3ffc8f7431fedc`
-	v2 Content-Length: 180.0 B
-	v2 Last-Modified: Fri, 06 May 2016 15:07:15 GMT

#### `8fd6fb866ea18ab6b5153616e91c4ea9b8b81a3349982b4118bfc347deedfa31`

```dockerfile
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data
```

-	Created: Wed, 04 May 2016 03:25:25 GMT
-	Parent Layer: `406a8b4a722c19cd18d2b048d0e425d1e487088eec44d1c0bbeb8d9ef5b7dd78`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `99f6ec6dca3cae4da6557e122d1acf201ea575cd5f110021d7411509ec0a81d7`

```dockerfile
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
```

-	Created: Wed, 04 May 2016 04:01:20 GMT
-	Parent Layer: `8fd6fb866ea18ab6b5153616e91c4ea9b8b81a3349982b4118bfc347deedfa31`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `40e9019ed184ba8b7b782147cbf8fa32110407807b94ee1d0162298badcd6a9e`

```dockerfile
ENV PHP_VERSION=5.6.21
```

-	Created: Wed, 04 May 2016 04:01:20 GMT
-	Parent Layer: `99f6ec6dca3cae4da6557e122d1acf201ea575cd5f110021d7411509ec0a81d7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `d532422949e5520306554a44dc4a2434ef7902cd8f1d31c5f30c85ca621c82a8`

```dockerfile
ENV PHP_FILENAME=php-5.6.21.tar.xz
```

-	Created: Wed, 04 May 2016 04:01:21 GMT
-	Parent Layer: `40e9019ed184ba8b7b782147cbf8fa32110407807b94ee1d0162298badcd6a9e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `560521cfa49cc2170168481c9890167d13ffb93931368f6da9db34a863288564`

```dockerfile
ENV PHP_SHA256=566ff1a486cb0485ed477a91ea292423f77a58671270ff73b74e67e3ce7084f9
```

-	Created: Wed, 04 May 2016 04:01:22 GMT
-	Parent Layer: `d532422949e5520306554a44dc4a2434ef7902cd8f1d31c5f30c85ca621c82a8`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `520f589892f775eda8a8649dc36fe8c94475094c1b3f7a5a7df404eee49eb55f`

```dockerfile
RUN set -xe \
	&& buildDeps=" \
		$PHP_EXTRA_BUILD_DEPS \
		libcurl4-openssl-dev \
		libedit-dev \
		libsqlite3-dev \
		libssl-dev \
		libxml2-dev \
		xz-utils \
	" \
	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME/from/this/mirror" -o "$PHP_FILENAME" \
	&& echo "$PHP_SHA256 *$PHP_FILENAME" | sha256sum -c - \
	&& curl -fSL "http://php.net/get/$PHP_FILENAME.asc/from/this/mirror" -o "$PHP_FILENAME.asc" \
	&& export GNUPGHOME="$(mktemp -d)" \
	&& for key in $GPG_KEYS; do \
		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; \
	done \
	&& gpg --batch --verify "$PHP_FILENAME.asc" "$PHP_FILENAME" \
	&& rm -r "$GNUPGHOME" "$PHP_FILENAME.asc" \
	&& mkdir -p /usr/src/php \
	&& tar -xf "$PHP_FILENAME" -C /usr/src/php --strip-components=1 \
	&& rm "$PHP_FILENAME" \
	&& cd /usr/src/php \
	&& ./configure \
		--with-config-file-path="$PHP_INI_DIR" \
		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" \
		$PHP_EXTRA_CONFIGURE_ARGS \
		--disable-cgi \
		--enable-mysqlnd \
		--enable-mbstring \
		--with-curl \
		--with-libedit \
		--with-openssl \
		--with-zlib \
	&& make -j"$(nproc)" \
	&& make install \
	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } \
	&& make clean \
	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false $buildDeps
```

-	Created: Wed, 04 May 2016 04:07:25 GMT
-	Parent Layer: `560521cfa49cc2170168481c9890167d13ffb93931368f6da9db34a863288564`
-	Docker Version: 1.9.1
-	Virtual Size: 136.3 MB (136300601 bytes)
-	v2 Blob: `sha256:2fa81675c8d53cfe31743f076e9ef9794aa52416ebc7f32a812921355e0ebc66`
-	v2 Content-Length: 26.5 MB (26473544 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:11:34 GMT

#### `efa109fb600faa91854b656c6bcd8b0721f7ce2e908c33dbb78bcf6697a7b87e`

```dockerfile
COPY multi:82b89724359b10e4fa6ed1d5d2d5ab38544995f1ed9288734f40288633831460 in /usr/local/bin/
```

-	Created: Wed, 04 May 2016 04:07:30 GMT
-	Parent Layer: `520f589892f775eda8a8649dc36fe8c94475094c1b3f7a5a7df404eee49eb55f`
-	Docker Version: 1.9.1
-	Virtual Size: 3.6 KB (3582 bytes)
-	v2 Blob: `sha256:2b9596305f8a7a19c2103e8bad0ada832f9d4ce0e3a16821c4627f0d0f102026`
-	v2 Content-Length: 1.5 KB (1548 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:11:07 GMT

#### `b29cd7954722ee9db9f0815315dda4487c009fb3d0f3c542fa9b1c274708ca65`

```dockerfile
WORKDIR /var/www/html
```

-	Created: Wed, 04 May 2016 04:07:31 GMT
-	Parent Layer: `efa109fb600faa91854b656c6bcd8b0721f7ce2e908c33dbb78bcf6697a7b87e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `438b852026867eb7dce1c48275da5a1dc4fa4b8809e170a3476dc119e6c1d95b`

```dockerfile
RUN set -ex \
	&& cd /usr/local/etc \
	&& if [ -d php-fpm.d ]; then \
		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; \
		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; \
	else \
		mkdir php-fpm.d; \
		cp php-fpm.conf.default php-fpm.d/www.conf; \
		{ \
			echo '[global]'; \
			echo 'include=etc/php-fpm.d/*.conf'; \
		} | tee php-fpm.conf; \
	fi \
	&& { \
		echo '[global]'; \
		echo 'error_log = /proc/self/fd/2'; \
		echo; \
		echo '[www]'; \
		echo '; if we send this to /proc/self/fd/1, it never appears'; \
		echo 'access.log = /proc/self/fd/2'; \
		echo; \
		echo 'clear_env = no'; \
		echo; \
		echo '; Ensure worker stdout and stderr are sent to the main error log.'; \
		echo 'catch_workers_output = yes'; \
	} | tee php-fpm.d/docker.conf \
	&& { \
		echo '[global]'; \
		echo 'daemonize = no'; \
		echo; \
		echo '[www]'; \
		echo 'listen = [::]:9000'; \
	} | tee php-fpm.d/zz-docker.conf
```

-	Created: Wed, 04 May 2016 04:07:33 GMT
-	Parent Layer: `b29cd7954722ee9db9f0815315dda4487c009fb3d0f3c542fa9b1c274708ca65`
-	Docker Version: 1.9.1
-	Virtual Size: 23.1 KB (23094 bytes)
-	v2 Blob: `sha256:dd763b7ae0fc69ad17ff4bdec9bc4e7dca77de0697e39cbb06d1daff1746f485`
-	v2 Content-Length: 7.7 KB (7683 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 15:11:01 GMT

#### `a399b1ebfc39b45da6a10012575dddb0ecc8555a83aa3890bcdf21fc62d30d92`

```dockerfile
EXPOSE 9000/tcp
```

-	Created: Wed, 04 May 2016 04:07:33 GMT
-	Parent Layer: `438b852026867eb7dce1c48275da5a1dc4fa4b8809e170a3476dc119e6c1d95b`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `fd19aeb28b3cfa77f4a99088bd64fe84019cec0533037123c7b07442e6957182`

```dockerfile
CMD ["php-fpm"]
```

-	Created: Wed, 04 May 2016 04:07:34 GMT
-	Parent Layer: `a399b1ebfc39b45da6a10012575dddb0ecc8555a83aa3890bcdf21fc62d30d92`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `84e75d5fcd801d02fb39b43bd527ee57d74b623b01fae8606da4a90f23fe9b3f`

```dockerfile
RUN apt-get update && apt-get install -y libpng12-dev libjpeg-dev && rm -rf /var/lib/apt/lists/* \
	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr \
	&& docker-php-ext-install gd mysqli opcache
```

-	Created: Thu, 05 May 2016 06:06:34 GMT
-	Parent Layer: `fd19aeb28b3cfa77f4a99088bd64fe84019cec0533037123c7b07442e6957182`
-	Docker Version: 1.9.1
-	Virtual Size: 14.7 MB (14685145 bytes)
-	v2 Blob: `sha256:0880dc1cc37191527670cff85823ae67dc87cb220d1eeb4a41adb67c163ae302`
-	v2 Content-Length: 4.4 MB (4420999 bytes)
-	v2 Last-Modified: Fri, 06 May 2016 23:38:48 GMT

#### `f639697e9e0ccb63766f00dfb552317abe9664bf82464c116cd890dc037d027e`

```dockerfile
RUN { \
		echo 'opcache.memory_consumption=128'; \
		echo 'opcache.interned_strings_buffer=8'; \
		echo 'opcache.max_accelerated_files=4000'; \
		echo 'opcache.revalidate_freq=60'; \
		echo 'opcache.fast_shutdown=1'; \
		echo 'opcache.enable_cli=1'; \
	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
```

-	Created: Thu, 05 May 2016 06:06:36 GMT
-	Parent Layer: `84e75d5fcd801d02fb39b43bd527ee57d74b623b01fae8606da4a90f23fe9b3f`
-	Docker Version: 1.9.1
-	Virtual Size: 172.0 B
-	v2 Blob: `sha256:cc9ba5c37fd237eb001a3fc70b1d43a8ad4732529b4a19eb8e3cdd00956013cf`
-	v2 Content-Length: 333.0 B
-	v2 Last-Modified: Fri, 06 May 2016 23:38:43 GMT

#### `bc1341fe62662a25cf97c82d3d2c6c3e1a1e360fd8ba3b18bce1fc07b81f6da7`

```dockerfile
VOLUME [/var/www/html]
```

-	Created: Thu, 05 May 2016 06:06:37 GMT
-	Parent Layer: `f639697e9e0ccb63766f00dfb552317abe9664bf82464c116cd890dc037d027e`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `3508ddf1c8913c5591dc5ca7361006d3adfb4c4278346293a07d868efc3fb871`

```dockerfile
ENV WORDPRESS_VERSION=4.5.2
```

-	Created: Tue, 10 May 2016 01:29:57 GMT
-	Parent Layer: `bc1341fe62662a25cf97c82d3d2c6c3e1a1e360fd8ba3b18bce1fc07b81f6da7`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `9a38934c092657f835f3042b4f56c8bca813f2b991d9fff26b8f8e9147aa07ca`

```dockerfile
ENV WORDPRESS_SHA1=bab94003a5d2285f6ae76407e7b1bbb75382c36e
```

-	Created: Tue, 10 May 2016 01:29:57 GMT
-	Parent Layer: `3508ddf1c8913c5591dc5ca7361006d3adfb4c4278346293a07d868efc3fb871`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `b72c4991df3200068f40a98e47d1ff0e9f5c94170c3c3a71012bef1603fcb994`

```dockerfile
RUN curl -o wordpress.tar.gz -SL https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz \
	&& echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c - \
	&& tar -xzf wordpress.tar.gz -C /usr/src/ \
	&& rm wordpress.tar.gz \
	&& chown -R www-data:www-data /usr/src/wordpress
```

-	Created: Tue, 10 May 2016 01:29:59 GMT
-	Parent Layer: `9a38934c092657f835f3042b4f56c8bca813f2b991d9fff26b8f8e9147aa07ca`
-	Docker Version: 1.9.1
-	Virtual Size: 21.9 MB (21908610 bytes)
-	v2 Blob: `sha256:817016e1ab05a17b14fc1abea031b00439450cd6f47e68cf84032582aa92bcef`
-	v2 Content-Length: 7.6 MB (7610170 bytes)
-	v2 Last-Modified: Tue, 10 May 2016 01:56:47 GMT

#### `1b78f1bff6be5744b7ed32aa5e86f3bbe0c743bfea2e7cb7b33d88c272694002`

```dockerfile
COPY file:e4f27140dddd16cd34ce106cb7587b487bdf49693a3436dc23a89fcb0f933d05 in /entrypoint.sh
```

-	Created: Thu, 12 May 2016 19:24:58 GMT
-	Parent Layer: `b72c4991df3200068f40a98e47d1ff0e9f5c94170c3c3a71012bef1603fcb994`
-	Docker Version: 1.9.1
-	Virtual Size: 5.2 KB (5155 bytes)
-	v2 Blob: `sha256:f79a39a56bc213acb9b5131bb94562383aecb31e2c72086fafd6aa36a9617201`
-	v2 Content-Length: 2.5 KB (2492 bytes)
-	v2 Last-Modified: Thu, 12 May 2016 20:00:20 GMT

#### `a2e083a2d07a138c1f313a0f22155f1a2c8734dca13c643a7a9ae543bc7b6295`

```dockerfile
ENTRYPOINT &{["/entrypoint.sh"]}
```

-	Created: Thu, 12 May 2016 19:24:58 GMT
-	Parent Layer: `1b78f1bff6be5744b7ed32aa5e86f3bbe0c743bfea2e7cb7b33d88c272694002`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT

#### `fa2fb79917c7b14115b62924f251fdc3cca863b981948cf9b95214f74f11ad07`

```dockerfile
CMD ["php-fpm"]
```

-	Created: Thu, 12 May 2016 19:24:59 GMT
-	Parent Layer: `a2e083a2d07a138c1f313a0f22155f1a2c8734dca13c643a7a9ae543bc7b6295`
-	Docker Version: 1.9.1
-	Virtual Size: 0.0 B
-	v2 Blob: `sha256:a3ed95caeb02ffe68cdd9fd84406680ae93d633cb16422d00e8a7c22955b46d4`
-	v2 Content-Length: 32.0 B
-	v2 Last-Modified: Sat, 14 Nov 2015 09:09:44 GMT
