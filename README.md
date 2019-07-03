# tslint-config

Quick and easy tslint config

Includes 3 configurations

-   Core
-   Core + RxJS
-   Core + RxJS + Angular

> Please note, that peer dependencies are not listed in `package.json` for RxJS and Angular configurations.
>
> You will not see the peer dependency warning if you are missing these dependencies when installing this package, but
> they must be installed if you are using those configurations.

## Installation

#### Core

`npm i -D tslint @quick-foot/tslint-config`

#### Core + RxJS

`npm i -D tslint @quick-foot/tslint-config rxjs rxjs-tslint-rules`

#### Core + RxJS + Angular

`npm i -D tslint @quick-foot/tslint-config rxjs rxjs-tslint-rules codelyzer @angular/compiler @angular/core`

## Usage

Ensure that you turn on strict mode in your `tsconfig.json`.

```json
{
    "compilerOptions": {
        "strict": true
    }
}
```

#### Core

`tslint.json`

```json
{
    "extends": "@quick-foot/tslint-config/core"
}
```

#### Core + RxJS

`tslint.json`

```json
{
    "extends": "@quick-foot/tslint-config/rxjs"
}
```

#### Core + RxJS + Angular

`tslint.json`

```json
{
    "extends": "@quick-foot/tslint-config/angular"
}
```

## Peer Dependency Requirements

#### Core

-   tslint @ >= 5.18.0
-   typescript @ >= 3.4.5

#### Core + RxJS

-   tslint @ >= 5.18.0
-   typescript @ >= 3.4.5
-   rxjs @ >= 6.5.2
-   rxjs-tslint-rules @ >= 4.24.3

#### Core + RxJS + Angular

-   tslint @ >= 5.18.0
-   typescript @ >= 3.4.5
-   rxjs @ >= 6.5.2
-   rxjs-tslint-rules @ >= 4.24.3
-   @angular/core @ >= 8.0.3
-   @angular/compiler @ >= 8.0.3
-   codelyzer @ >= 5.1.0
