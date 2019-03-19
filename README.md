# resolve-packages

Script to resolve npm package versions to commits.

## Usage

Setup dependencies (requires pipenv):

```
pipenv
```

To run on a specific package version (for `request@2.88.0`):

```
pipenv run python resolve_npm.py request 2.88.0
```

To download [most depended upon packages](https://www.npmjs.com/browse/depended) and run all:

```
pipenv run python resolve_npm.py
```

To run with GitHub PAT, set a environment variable `GITHUB_TOKEN` with the PAT, and then run the same script.

## Output

Example output on most depended upon packages (32/36 resolved):

```
lodash: 4.17.11 resolved to 0843bd46ef805dd03c0c8d804630804f3ba0ca3c
request: 2.88.0 resolved to 642024036379239a7fa29c27ef7bb4dd3fa3b3a4
chalk: 2.4.2 resolved to 9776a2ae5b5b1712ccf16416b55f47e575a81fb9
react: 16.8.4 resolved to d8a73b5eb6c7217850103193635ff1b556925ed5
express: 4.16.4 resolved to dc538f6e810bd462c98ee7e6aae24c64d4b1da93
commander: 2.19.0 resolved to 78b7dbd18aabc23ccc9d151db411913237a3c483
moment: 2.24.0 resolved to 96d0d6791ab495859d09a868803d31a55c917de1
async: 2.6.2 resolved to eaf32be0e94f62fddc83d8550814e30a4be66a3c
debug: 4.1.1 resolved to 68b4dc8d8549d3924673c38fccc5d594f0a38da1
bluebird: 3.5.3 resolved to 50bc72e561f55c4e4118988186516ee19d18cf28
prop-types: 15.7.2 resolved to 953ed9beb0f15498cd7e6e25c90f7cadd5f2149a
react-dom: 16.8.4 resolved to d8a73b5eb6c7217850103193635ff1b556925ed5
fs-extra: 7.0.1 resolved to a32c85282185aa008759890cce059594e4348262
underscore: 1.9.1 resolved to ae037f7c41323807ae6f1533c45512e6d31a1574
axios: 0.18.0 resolved to d59c70fdfd35106130e9f783d0dbdcddd145b58f
tslib: 1.9.3 resolved to 9dd9aa322c893e5e0b3f1609b1126314ccf37bbb
uuid: 3.3.2 resolved to fe4ae79c55af2c7cbf2bb39d3bcb6716d5367091
mkdirp: 0.5.1 resolved to d4eff0f06093aed4f387e88e9fc301cb76beedc7
classnames: found repo, cannot resolve 2.2.6 to commit
body-parser: 1.18.3 resolved to e6ccf98015fece0851c0c673fc2776c30ad79e5d
glob: 7.1.3 resolved to 8882c8fccabbe459465e73cc2581e121a5fdd25b
babel-runtime: found repo, cannot resolve 6.26.0 to commit
colors: 1.3.3 resolved to b63ef88e521b42920a9e908848de340b31e68c9d
yargs: 13.2.2 resolved to e7f29379707f9e3d5eb6edc09ba278f53cc7db74
webpack: 4.29.6 resolved to 685a0626cb10664133ef2fb2e2f9f4cb3971402a
rxjs: 6.4.0 resolved to d3e7e3f299e277b077602d26c59dab40ef0e1dba
vue: 2.6.9 resolved to 43115e09e98d484a35f7c12249396b6d5d66c7ff
jquery: 3.3.1 resolved to 32b00373b3f42e5cdcb709df53f3b08b7184a944
minimist: 1.2.0 resolved to dc624482fcfec5bc669c68cdb861f00573ed4e64
inquirer: found repo, cannot resolve 6.2.2 to commit
babel-core: found repo, cannot resolve 6.26.3 to commit
yeoman-generator: 3.2.0 resolved to 3bbeef0f8eebd02e9459734c9a3d9c6732a47d14
through2: 3.0.1 resolved to d0696e4be57337c5742ac6fe9d20892a2ab78b2e
aws-sdk: 2.423.0 resolved to aca7cf991add5fb7fcb98aebaf08edf421094a47
redux: 4.0.1 resolved to c5d87d95f3b9b0ebdb57791f69b53d8507cebbed
babel-loader: 8.0.5 resolved to 20c9e0eef9e62e7041a42c71509486cc44bbcb5a
```

Next 36 (33/36 resolved):

```
q: 1.5.1 resolved to c2f5a6f35456389a806acca50bfd929cbe30c4cb
winston: 3.2.1 resolved to 49ccdb6604ecce590eda2915b130970ee0f1b6a3
dotenv: 7.0.0 resolved to 72fb66b051280ef5c2cc40ce4962ac4601f7f515
semver: 5.6.0 resolved to 46727afbe21b8d14641a0d1c4c7ee58bd053f922
cheerio: 1.0.0-rc.2 resolved to 48eae25c93702a29b8cd0d09c4a2dce2f912d1f4
rimraf: 2.6.3 resolved to 9442819908e52f2c32620e8fa609d7a5d472cc2c
css-loader: 2.1.1 resolved to bc16c3db953dbf4d711753fbb0cc60253def6916
eslint: 5.15.3 resolved to a6168f85f9017332777b2bac5af8c4a979e06298
core-js: 2.6.5 resolved to e778e8026aed8a58f93f1ee4e3192cd1a7d7bdf5
@angular/core: 7.2.9 resolved to 5abb9360d822ad98a7905d11ff89e42e80050c6a
react-redux: 6.0.1 resolved to 162b81a3fffe75ff6181b711777067ba6e63a34b
typescript: 3.3.3333 resolved to b145eaf160e6b2729aaacb89856bc2346f85ac4c
shelljs: 0.8.3 resolved to d4d1317ce62531fbd49085852b8492db3dd39312
style-loader: 0.23.1 resolved to 80039665d612248535557c41de03a5aa377484a8
@types/node: repository url not resolved
@angular/common: 7.2.9 resolved to 5abb9360d822ad98a7905d11ff89e42e80050c6a
js-yaml: 3.12.2 resolved to e4267fc733452d074a3e494fb5cab2a07c7e6b87
zone.js: 0.8.29 resolved to ce9c2e056e1393e2d5e01be688f4cbf6d174ce15
object-assign: 4.1.1 resolved to a89774b252c91612203876984bbd6addbe3b5a0e
gulp: 4.0.0 resolved to 55eb23a268dcc7340bb40808600fd4802848c06f
babel-polyfill: found repo, cannot resolve 6.26.0 to commit
ramda: 0.26.1 resolved to 6709cb8beca00178d2288f79568cc5ca9e95d2f5
babel-preset-es2015: found repo, cannot resolve 6.24.1 to commit
babel-eslint: 10.0.1 resolved to 4cf0a21a4b12e64ce4012bbfcc62d0d969053f8b
gulp-util: 3.0.8 resolved to 28c2aa2a3f8782a995b47ed051ab52885c705024
@angular/platform-browser: 7.2.9 resolved to 5abb9360d822ad98a7905d11ff89e42e80050c6a
file-loader: 3.0.1 resolved to 011cc38d4ed470729ff0fbc6c1d7146896603598
request-promise: 4.2.4 resolved to 4e3b7ed87ae9a120aae2c4613e93aec3f8a615a9
node-fetch: 2.3.0 resolved to 5367fe6a978e01745e4264384a91140dc99a4bf8
mongoose: 5.4.19 resolved to 5e47d8be8b35599e4997d5f2ef88ef19c7853a32
@angular/compiler: 7.2.9 resolved to 5abb9360d822ad98a7905d11ff89e42e80050c6a
handlebars: 4.1.1 resolved to f691db546e7563e1db3437d5a72f478f9e556714
mocha: 6.0.2 resolved to 00a895f6ad9c1e4c5500851d6ff875e8254a5e06
mongodb: 3.1.13 resolved to c6f417e5fe54691783bccc466e7703a5d380739e
@angular/forms: 7.2.9 resolved to 5abb9360d822ad98a7905d11ff89e42e80050c6a
@angular/platform-browser-dynamic: 7.2.9 resolved to 5abb9360d822ad98a7905d11ff89e42e80050c6a
```
