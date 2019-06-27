---
title: Microsoft Graph ツールキットプロバイダー
description: Microsoft Graph Toolkit プロバイダーを使用すると、すべてのコンポーネントに対して認証と Microsoft Graph へのアクセスが可能になります。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e89247daf92471b4a7c6aa16f34396eaedaaa37a
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243059"
---
# <a name="microsoft-graph-toolkit-providers"></a>Microsoft Graph ツールキットプロバイダー

Microsoft Graph Toolkit プロバイダーを使用すると、すべてのコンポーネントに対して認証と Microsoft Graph へのアクセスが可能になります。 各プロバイダーは、Microsoft Graph Api を呼び出すために必要なアクセストークンを取得するための実装を提供します。

コンポーネントでプロバイダーを使用するには、使用するプロバイダー `Providers.globalProvider`の値をプロパティに設定する必要があります。

次の例は、MsalProvider の使用方法を示しています。

```js
Providers.globalProvider = new MsalProvider({
  clientId: '[CLIENT_ID]'
});
```

このツールキットは、次のプロバイダーを実装します。

- [MsalProvider](./providers/msal.md)
- [SharePointProvider](./providers/sharepoint.md)
- [TeamsProvider](./providers/teams.md)
- Office アドインプロバイダー (近日公開予定)

## <a name="get-started"></a>作業の開始

プロバイダーはいつでも作成できます。 コンポーネントを使用する前に、プロバイダーを作成することをお勧めします。 このセクションでは、プロバイダーを初期化する方法について説明します。

グローバル`Providers`変数は、次のプロパティと関数を公開します。

   - `globalProvider : IProvider`

このプロパティをグローバルに使用するプロバイダーに設定します。 すべてのコンポーネントこのプロパティを使用して、プロバイダーへの参照を取得します。 このプロパティを設定すると`onProvidersChanged` 、イベントが発生します。

   - `function onProviderUpdated(callbackFunction)`

 この`callbackFunction`関数は、プロバイダーが変更されたとき、またはプロバイダーの状態が変更されたときに呼び出されます。 `ProvidersChangedState`列挙値は、更新されたものを示すために関数に渡されます。

## <a name="implement-your-own-provider"></a>独自のプロバイダーを実装する

このツールキットには、新しいプロバイダーを作成する2つの方法が用意されています。

- アクセストークンを`SimpleProvider`取得するために関数を渡すことにより、新しいを作成する
- 抽象クラス`IProvider`を拡張する

詳細については、「[カスタムプロバイダー](./providers/custom.md) 」のドキュメントの「」を参照してください。

## <a name="making-your-own-calls-to-microsoft-graph"></a>Microsoft Graph への独自の呼び出しを行う

すべてのコンポーネントは、前のセクションで説明したように、プロバイダーを初期化する限り、カスタマイズを必要とせずに Microsoft Graph にアクセスできます。 コンポーネントで使用されているものと同じ Microsoft Graph SDK への参照を取得するには、まず、グローバル IProvider へ`Graph`の参照を取得してから、そのオブジェクトを使用します。次に示します。

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```

呼び出している API によっては、追加のアクセス許可を渡す必要がある場合があります。

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

`graph`オブジェクトは、 [MICROSOFT graph Javascript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript)のインスタンスであり、これを使用して microsoft graph へのすべての呼び出しを行うことができます。
