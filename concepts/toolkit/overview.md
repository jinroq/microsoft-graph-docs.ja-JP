---
title: Microsoft Graph Toolkit (プレビュー)
description: Microsoft Graph Toolkit は、フレームワークに依存しない web コンポーネントと、Microsoft Graph にアクセスして作業するためのヘルパーのコレクションです。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e6d5974029625a8dd1bef0c7b981fcf2b36b747c
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243063"
---
# <a name="microsoft-graph-toolkit-preview"></a>Microsoft Graph Toolkit (プレビュー)

Microsoft Graph Toolkit は、フレームワークに依存しない web コンポーネントと、Microsoft Graph にアクセスして作業するためのヘルパーのコレクションです。 すべてのコンポーネントは、カスタマイズを必要とせずに Microsoft Graph にアクセスできます。

>[!NOTE]
>このライブラリはプレビュー版で、初期段階の開発に含まれています。 コミュニティからのフィードバックに基づいて、すべてのコンポーネントと Api に変更が加えられ、強化されることを期待しています。

## <a name="get-started"></a>作業の開始

コンポーネントを使用するには、そのローダーを直接 (または、pkg を介して) 参照するか、または npm パッケージをインストールします。

Microsoft Graph Toolkit を使用して作業を開始する方法の詳細については、「はじめに」の[ビデオ](https://www.youtube.com/watch?v=oZCGb2MMxa0)を参照してください。

### <a name="use-via-mgt-loader"></a>Via による使用-ローダー

[次の jsfiddle 例](https://jsfiddle.net/metulev/9phqxLd5/)を参照してください。

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

その後、HTML ページのコンポーネントの使用を開始できます。 以下に、MSAL プロバイダーを使用した完全な作業例を示します。

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
<mgt-login></mgt-login>

<!-- <script>
    // alternatively, you can set the provider in code and provide more options
    mgt.Providers.globalProvider = new mgt.MsalProvider({clientId: '[CLIENT-ID]'});
</script> -->
```

> **注:** MSAL では、認証リダイレクト用に web サーバーでページをホストする必要があります。 すぐにプレイしたい場合は、Visual Studio Code で[live サーバー](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)を使用することができます。

### <a name="use-via-npm-es6-modules"></a>NPM 経由で使用する (es6 モジュール)

Es6 モジュールを使用すると、バンドル処理を完全に制御でき、サイトに必要なコードのみをバンドルできます。 最初に、npm パッケージを追加します。

```bash
npm install @microsoft/mgt
```

これで、使用しているページのすべてのコンポーネントを参照できるようになりました。

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

または、必要なコンポーネントを参照するだけで、それ以外のすべての読み込みが行われないようにします。

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

同様に、プロバイダーを追加するには、それをコンポーネントとして追加します。

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>

<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
```

または、コードに追加します。

```html
<script type="module">
  import { Providers, MsalProvider } from '@microsoft/mgt';

  Providers.globalProvider = new MsalProvider({ clientId: '[CLIENT-ID]' });
</script>
```

## <a name="providers"></a>会社

コンポーネントは、[プロバイダー](./providers.md)で使用する場合に最適に機能します。 プロバイダーは、コンポーネントが Microsoft Graph を呼び出すために使用する認証と Api を公開します。

ツールキットには、 [Msal](./providers/msal.md)、 [SharePoint](./providers/sharepoint.md)、 [Teams](./providers/teams.md)、Office アドインのプロバイダーが含まれています (近日中)。 [IProvider] 抽象クラスを拡張して、独自のプロバイダーを作成することもできます。

## <a name="polyfills"></a>Polyfills.ts

Npm パッケージの es6 モジュールを使用している場合は、polyfills.ts が自動的に含まれないように、プロジェクトにを含めるようにしてください。 詳細については、「 [polyfills.ts](https://www.webcomponents.org/polyfills)」を参照してください。

Mgt-loader スクリプトをパッケージ化されていないパッケージから使用している場合、polyfills.ts は既に含まれています。


## <a name="using-the-components-with-react-angular-and-other-frameworks"></a>コンポーネントを反応、角度、およびその他のフレームワークで使用する

Web コンポーネントは、いくつかの web 標準に基づいており、既に使用しているフレームワークで使用できます。 ただし、すべてのフレームワークが web コンポーネントを同じ方法で処理するわけではありません。 フレームワークに応じて適用される可能性のある考慮事項の詳細については、「すべての場所のプロジェクトに[カスタム要素](https://custom-elements-everywhere.com/)を表示する」を参照してください。

次のセクションでは、Microsoft Graph のツールキットコンポーネントを使用して、反応があり、角度を指定する方法の概要を簡単に説明します。

### <a name="react"></a>React

応答は、すべてのデータを HTML 属性の形式でカスタム要素に渡します。 プリミティブデータの場合、これは問題ありませんが、オブジェクトや配列などの豊富なデータを渡すときには動作しません。 そのような場合は、 `ref`を使用してオブジェクトを渡す必要があります。

渡し

```jsx
// import all the components
import '@microsoft/mgt';

class App extends Component {
  render() {
    return <mgt-person show-name ref={el => (el.personDetails = { displayName: 'Nikola Metulev' })} />;
  }
}
```

応答は独自の代理イベントシステムを実装するため、回避策を使用せずにカスタム要素からの DOM イベントをリッスンすることはできません。 次の例に示すよう`ref`に、を使用して、ツールキットコンポーネントを参照し、イベントリスナーを addEventListener で手動でアタッチする必要があります。

```jsx
// you can just import a single component
import '@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js';

class App extends Component {
  render() {
    return <mgt-login ref="loginComponent" />;
  }

  componentDidMount() {
    this.refs.loginComponent.addEventListener('loginCompleted', e => {
      // handle event
    });
  }
}
```

#### <a name="react-typescript-and-tsx"></a>反応、Typescript、および TSX

対応および Typescript でカスタム要素を使用すると、既知の問題が発生することがあります。 Tsx でコンポーネントを使用しようとすると、Typescript によってエラーがスローされます。 回避策は、コードでカスタム要素を定義することです。以下に例を示します。

```ts
declare global {
  namespace JSX {
    interface IntrinsicElements {
      'mgt-login': any;
    }
  }
}
```

その後、を tsx で使用でき`<mgt-login></mgt-login>`ます。

### <a name="angular"></a>Angular

角度の既定のバインド構文は、常に要素のプロパティを設定します。 これは、オブジェクトや配列などの豊富なデータに適しています。また、プリミティブ値にも適しています。

カスタム要素を使用するには、まず、 `app.module.ts` `CUSTOM_ELEMENT_SCHEMA`を`@NgModule() decorator`に追加して、でカスタム要素を有効にします。次に例を示します。

```ts
import { BrowserModule } from '@angular/platform-browser';
import { NgModule, CUSTOM_ELEMENTS_SCHEMA } from '@angular/core';

import { AppComponent } from './app.component';

@NgModule({
  declarations: [AppComponent],
  imports: [BrowserModule],
  schemas: [CUSTOM_ELEMENTS_SCHEMA],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule {}
```

その後、コンポーネント\*の ts ファイルで使用するコンポーネントをインポートできます。

```ts
import { Component } from '@angular/core';
import '@microsoft/mgt/dist/es6/components/mgt-person/mgt-person';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  person = {
    displayName: 'Nikola Metulev'
  };
}
```

最後に、テンプレート内の通常のようにコンポーネントを使用します。

```html
<mgt-person [personDetails]="person" show-name></mgt-person>
```
