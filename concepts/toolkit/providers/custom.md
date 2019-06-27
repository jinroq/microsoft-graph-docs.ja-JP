---
title: カスタムプロバイダー
description: アプリケーションに既存の認証コードがある場合は、Microsoft Graph Toolkit コンポーネントの認証とグラフアクセスを有効にするためのカスタムプロバイダーを作成します。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: acd96e6dc7e13b1e1fbfc5353e3db2132a23e246
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243053"
---
# <a name="custom-provider"></a>カスタムプロバイダー

アプリケーションに既存の認証コードがある場合は、カスタムプロバイダーを作成して、Microsoft Graph Toolkit コンポーネントの認証と Microsoft Graph へのアクセスを有効にすることができます。 カスタムプロバイダーを作成するには、次の2つの方法があります。

- アクセストークンを`SimpleProvider`取得するために関数を渡すことにより、新しいを作成する
- 抽象クラス`IProvider`を拡張する

この記事では、各方法について詳しく説明します。

## <a name="simpleprovider"></a>SimpleProvider

渡され`SimpleProvider`たスコープのアクセストークンを返す関数を渡すことにより、クラスをインスタンス化します。

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

さらに、[ログイン](../components/login.md)コンポーネントからのサインインと`login`サインアウト`logout`の呼び出しを処理できるオプションおよび関数を提供することもできます。

```ts
function getAccessToken(scopes: string[]) {
  // return a promise with accessToken string
}

function login() {
  // login code
}

function logout() {
  // logout code
}

let provider = new SimpleProvider(getAccessToken, login, logout);
```

### <a name="manage-state"></a>状態を管理する

プロバイダーの状態を認識できるようにコンポーネントを構成するには、状態が変化し`provider.setState(state: ProviderState)`たときにメソッドを呼び出す必要があります。 たとえば、ユーザーがサインインしている場合は、 `provider.setState(ProviderState.SignedIn)`を呼び出します。 Enum `ProviderState`は、次のように3つの状態を定義します。

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a>IProvider

`IProvider`抽象クラスを拡張して、独自のプロバイダーを作成できます。

### <a name="state"></a>State

プロバイダーは、認証状態を追跡し、状態が変更されたときにコンポーネントを更新する必要があります。 `IProvider`クラスには、 `onStateChanged(eventHandler)`ハンドラーと`state: ProviderState`プロパティが既に実装されています。 変更時に状態を更新`setState(state:ProviderState)`するには、実装のメソッドを使用するだけです。 状態を更新すると、 `stateChanged`イベントが発生し、すべてのコンポーネントが自動的に更新されます。

### <a name="loginlogout"></a>ログイン/ログアウト

プロバイダーがログインまたはログアウト機能を提供する場合`login(): Promise<void>`は`logout(): Promise<void>` 、メソッドとメソッドを実装します。 これらのメソッドはオプションです。

### <a name="access-token"></a>アクセストークン

`getAccessToken({'scopes': scopes[]}) : Promise<string>`メソッドを実装する必要があります。 このメソッドは、Microsoft Graph へのすべての呼び出しの前に有効なトークンを取得するために使用されます。

### <a name="graph"></a>反転

これらのコンポーネントは、microsoft graph のすべての呼び出しに Microsoft Graph Javascript SDK を使用します。 プロバイダーは、 `graph`プロパティで SDK を使用できるようにする必要があります。 のように、コンストラクターで新しい`Graph`インスタンスを作成します。

```js
this.graph = new Graph(this);
```

`Graph`クラスは、MICROSOFT Graph SDK の一番上にあるライトラッパーです。

### <a name="example"></a>例

すべてのプロバイダーが抽象`IProvider`クラスを拡張します。 例については、[既存のプロバイダー](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/src/providers)のソースコードを参照してください。

## <a name="set-the-global-provider"></a>グローバルプロバイダーを設定する

コンポーネントは、 `Providers.globalProvider`プロパティを使用してプロバイダーにアクセスします。 独自のプロバイダーを作成した後、このプロパティをプロバイダーに設定します。

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

すべてのコンポーネントは新しいプロバイダーに通知され、その使用を開始します。
