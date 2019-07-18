---
title: Microsoft Graph ツールキットプロバイダー
description: Microsoft Graph Toolkit プロバイダーを使用すると、すべてのコンポーネントに対して認証と Microsoft Graph へのアクセスが可能になります。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 3e5d587e8c2690d2b71a2e70e41266519566f91e
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778713"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="b2bad-103">Microsoft Graph ツールキットプロバイダー</span><span class="sxs-lookup"><span data-stu-id="b2bad-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="b2bad-104">Microsoft Graph Toolkit プロバイダーを使用すると、すべてのコンポーネントに対して認証と Microsoft Graph へのアクセスが可能になります。</span><span class="sxs-lookup"><span data-stu-id="b2bad-104">The Microsoft Graph Toolkit providers enable authentication and Microsoft Graph access for all components.</span></span> <span data-ttu-id="b2bad-105">各プロバイダーは、Microsoft Graph Api を呼び出すために必要なアクセストークンを取得するための実装を提供します。</span><span class="sxs-lookup"><span data-stu-id="b2bad-105">Each provider provides implementation for acquiring the necessary access token for calling the Microsoft Graph APIs.</span></span>

<span data-ttu-id="b2bad-106">コンポーネントでプロバイダーを使用するには、使用するプロバイダー `Providers.globalProvider`の値をプロパティに設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2bad-106">For the components to use a provider, you must set the `Providers.globalProvider` property to the value for a provider you'd like to use.</span></span>

<span data-ttu-id="b2bad-107">次の例は、MsalProvider の使用方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="b2bad-107">The following example shows how to use the MsalProvider.</span></span>

```js
Providers.globalProvider = new MsalProvider({
  clientId: '[CLIENT_ID]'
});
```

<span data-ttu-id="b2bad-108">このツールキットは、次のプロバイダーを実装します。</span><span class="sxs-lookup"><span data-stu-id="b2bad-108">The toolkit implements the following providers:</span></span>

- [<span data-ttu-id="b2bad-109">MsalProvider</span><span class="sxs-lookup"><span data-stu-id="b2bad-109">MsalProvider</span></span>](./providers/msal.md)
- [<span data-ttu-id="b2bad-110">SharePointProvider</span><span class="sxs-lookup"><span data-stu-id="b2bad-110">SharePointProvider</span></span>](./providers/sharepoint.md)
- [<span data-ttu-id="b2bad-111">TeamsProvider</span><span class="sxs-lookup"><span data-stu-id="b2bad-111">TeamsProvider</span></span>](./providers/teams.md)
- <span data-ttu-id="b2bad-112">Office アドインプロバイダー (近日公開予定)</span><span class="sxs-lookup"><span data-stu-id="b2bad-112">Office Add-ins provider (coming soon)</span></span>

## <a name="get-started"></a><span data-ttu-id="b2bad-113">作業の開始</span><span class="sxs-lookup"><span data-stu-id="b2bad-113">Get started</span></span>

<span data-ttu-id="b2bad-114">プロバイダーはいつでも作成できます。</span><span class="sxs-lookup"><span data-stu-id="b2bad-114">You can create a provider at any time.</span></span> <span data-ttu-id="b2bad-115">コンポーネントを使用する前に、プロバイダーを作成することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="b2bad-115">We recommend that you create the provider before you use any of the components.</span></span> <span data-ttu-id="b2bad-116">このセクションでは、プロバイダーを初期化する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="b2bad-116">This section describes how to initialize a provider.</span></span>

<span data-ttu-id="b2bad-117">グローバル`Providers`変数は、次のプロパティと関数を公開します。</span><span class="sxs-lookup"><span data-stu-id="b2bad-117">The `Providers` global variable exposes the following properties and functions</span></span>

- `globalProvider : IProvider`

<span data-ttu-id="b2bad-118">このプロパティをグローバルに使用するプロバイダーに設定します。</span><span class="sxs-lookup"><span data-stu-id="b2bad-118">Set this property to a provider that you want to use globally.</span></span> <span data-ttu-id="b2bad-119">すべてのコンポーネントこのプロパティを使用して、プロバイダーへの参照を取得します。</span><span class="sxs-lookup"><span data-stu-id="b2bad-119">All components use this property to get a reference to the provider.</span></span> <span data-ttu-id="b2bad-120">このプロパティを設定すると`onProvidersChanged` 、イベントが発生します。</span><span class="sxs-lookup"><span data-stu-id="b2bad-120">Setting this property will fire the `onProvidersChanged` event.</span></span>

- `function onProviderUpdated(callbackFunction)`

<span data-ttu-id="b2bad-121">この`callbackFunction`関数は、プロバイダーが変更されたとき、またはプロバイダーの状態が変更されたときに呼び出されます。</span><span class="sxs-lookup"><span data-stu-id="b2bad-121">The `callbackFunction` function will be called when a provider is changed or when the state of a provider changes.</span></span> <span data-ttu-id="b2bad-122">`ProvidersChangedState`列挙値は、更新されたものを示すために関数に渡されます。</span><span class="sxs-lookup"><span data-stu-id="b2bad-122">A `ProvidersChangedState` enum value will be passed to the function to indicate what updated.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="b2bad-123">独自のプロバイダーを実装する</span><span class="sxs-lookup"><span data-stu-id="b2bad-123">Implement your own provider</span></span>

<span data-ttu-id="b2bad-124">このツールキットには、新しいプロバイダーを作成する2つの方法が用意されています。</span><span class="sxs-lookup"><span data-stu-id="b2bad-124">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="b2bad-125">アクセストークンを`SimpleProvider`取得するために関数を渡すことにより、新しいを作成する</span><span class="sxs-lookup"><span data-stu-id="b2bad-125">Create a new `SimpleProvider` by passing in a function for getting an access token</span></span>
- <span data-ttu-id="b2bad-126">抽象クラス`IProvider`を拡張する</span><span class="sxs-lookup"><span data-stu-id="b2bad-126">Extend the `IProvider` abstract class</span></span>

<span data-ttu-id="b2bad-127">詳細については、「[カスタムプロバイダー](./providers/custom.md) 」のドキュメントの「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b2bad-127">Read more about each one in the [custom providers](./providers/custom.md) documentation.</span></span>

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="b2bad-128">Microsoft Graph への独自の呼び出しを行う</span><span class="sxs-lookup"><span data-stu-id="b2bad-128">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="b2bad-129">すべてのコンポーネントは、前のセクションで説明したように、プロバイダーを初期化する限り、カスタマイズを必要とせずに Microsoft Graph にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b2bad-129">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous section).</span></span> <span data-ttu-id="b2bad-130">コンポーネントで使用されているものと同じ Microsoft Graph SDK への参照を取得するには、まず、グローバル IProvider へ`Graph`の参照を取得してから、そのオブジェクトを使用します。次に示します。</span><span class="sxs-lookup"><span data-stu-id="b2bad-130">To get a reference to the same Microsoft Graph SDK used by the components, first get a reference to the global IProvider and then use the `Graph` object, as shown.</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```

<span data-ttu-id="b2bad-131">呼び出している API によっては、追加のアクセス許可を渡す必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="b2bad-131">There might be cases were you will need to pass additional permissions, depending on the API you're calling.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

<span data-ttu-id="b2bad-132">`graph`オブジェクトは、 [MICROSOFT graph Javascript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript)のインスタンスであり、これを使用して microsoft graph へのすべての呼び出しを行うことができます。</span><span class="sxs-lookup"><span data-stu-id="b2bad-132">The `graph` object is an instance of the [Microsoft Graph Javascript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) and you can use it to make any calls to Microsoft Graph.</span></span>
