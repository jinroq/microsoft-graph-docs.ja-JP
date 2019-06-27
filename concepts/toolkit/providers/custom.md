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
# <a name="custom-provider"></a><span data-ttu-id="61f62-103">カスタムプロバイダー</span><span class="sxs-lookup"><span data-stu-id="61f62-103">Custom provider</span></span>

<span data-ttu-id="61f62-104">アプリケーションに既存の認証コードがある場合は、カスタムプロバイダーを作成して、Microsoft Graph Toolkit コンポーネントの認証と Microsoft Graph へのアクセスを有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="61f62-104">If you have existing authentication code in your application, you can create a custom provider to enable authentication and access to Microsoft Graph for Microsoft Graph Toolkit components.</span></span> <span data-ttu-id="61f62-105">カスタムプロバイダーを作成するには、次の2つの方法があります。</span><span class="sxs-lookup"><span data-stu-id="61f62-105">There are two ways to create custom providers:</span></span>

- <span data-ttu-id="61f62-106">アクセストークンを`SimpleProvider`取得するために関数を渡すことにより、新しいを作成する</span><span class="sxs-lookup"><span data-stu-id="61f62-106">Create a new `SimpleProvider` by passing in a function for getting an access token</span></span>
- <span data-ttu-id="61f62-107">抽象クラス`IProvider`を拡張する</span><span class="sxs-lookup"><span data-stu-id="61f62-107">Extend the `IProvider` abstract class</span></span>

<span data-ttu-id="61f62-108">この記事では、各方法について詳しく説明します。</span><span class="sxs-lookup"><span data-stu-id="61f62-108">This article describes each approach in more detail.</span></span>

## <a name="simpleprovider"></a><span data-ttu-id="61f62-109">SimpleProvider</span><span class="sxs-lookup"><span data-stu-id="61f62-109">SimpleProvider</span></span>

<span data-ttu-id="61f62-110">渡され`SimpleProvider`たスコープのアクセストークンを返す関数を渡すことにより、クラスをインスタンス化します。</span><span class="sxs-lookup"><span data-stu-id="61f62-110">Instantiate the `SimpleProvider` class by passing in a function that will return an access token for passed-in scopes.</span></span>

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

<span data-ttu-id="61f62-111">さらに、[ログイン](../components/login.md)コンポーネントからのサインインと`login`サインアウト`logout`の呼び出しを処理できるオプションおよび関数を提供することもできます。</span><span class="sxs-lookup"><span data-stu-id="61f62-111">In addition, you can also provide an optional `login` and `logout` functions that can handle the sign in and sign out calls from the [Login](../components/login.md) component.</span></span>

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

### <a name="manage-state"></a><span data-ttu-id="61f62-112">状態を管理する</span><span class="sxs-lookup"><span data-stu-id="61f62-112">Manage state</span></span>

<span data-ttu-id="61f62-113">プロバイダーの状態を認識できるようにコンポーネントを構成するには、状態が変化し`provider.setState(state: ProviderState)`たときにメソッドを呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="61f62-113">For the components to be aware of the state of the provider, you will need to call the `provider.setState(state: ProviderState)` method whenever the state changes.</span></span> <span data-ttu-id="61f62-114">たとえば、ユーザーがサインインしている場合は、 `provider.setState(ProviderState.SignedIn)`を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="61f62-114">For example, when the user has signed in, call `provider.setState(ProviderState.SignedIn)`.</span></span> <span data-ttu-id="61f62-115">Enum `ProviderState`は、次のように3つの状態を定義します。</span><span class="sxs-lookup"><span data-stu-id="61f62-115">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a><span data-ttu-id="61f62-116">IProvider</span><span class="sxs-lookup"><span data-stu-id="61f62-116">IProvider</span></span>

<span data-ttu-id="61f62-117">`IProvider`抽象クラスを拡張して、独自のプロバイダーを作成できます。</span><span class="sxs-lookup"><span data-stu-id="61f62-117">You can extend the `IProvider` abstract class to create your own provider.</span></span>

### <a name="state"></a><span data-ttu-id="61f62-118">State</span><span class="sxs-lookup"><span data-stu-id="61f62-118">State</span></span>

<span data-ttu-id="61f62-119">プロバイダーは、認証状態を追跡し、状態が変更されたときにコンポーネントを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="61f62-119">A provider must keep track of the authentication state and update the components when the state changes.</span></span> <span data-ttu-id="61f62-120">`IProvider`クラスには、 `onStateChanged(eventHandler)`ハンドラーと`state: ProviderState`プロパティが既に実装されています。</span><span class="sxs-lookup"><span data-stu-id="61f62-120">The `IProvider` class already implements the `onStateChanged(eventHandler)` handler and the `state: ProviderState` property.</span></span> <span data-ttu-id="61f62-121">変更時に状態を更新`setState(state:ProviderState)`するには、実装のメソッドを使用するだけです。</span><span class="sxs-lookup"><span data-stu-id="61f62-121">You just need to use the `setState(state:ProviderState)` method in your implementation to update the state when it changes.</span></span> <span data-ttu-id="61f62-122">状態を更新すると、 `stateChanged`イベントが発生し、すべてのコンポーネントが自動的に更新されます。</span><span class="sxs-lookup"><span data-stu-id="61f62-122">Updating the state will fire the `stateChanged` event and update all the components automatically.</span></span>

### <a name="loginlogout"></a><span data-ttu-id="61f62-123">ログイン/ログアウト</span><span class="sxs-lookup"><span data-stu-id="61f62-123">Login/Logout</span></span>

<span data-ttu-id="61f62-124">プロバイダーがログインまたはログアウト機能を提供する場合`login(): Promise<void>`は`logout(): Promise<void>` 、メソッドとメソッドを実装します。</span><span class="sxs-lookup"><span data-stu-id="61f62-124">If your provider provides login or logout functionality, implement the `login(): Promise<void>` and `logout(): Promise<void>` methods.</span></span> <span data-ttu-id="61f62-125">これらのメソッドはオプションです。</span><span class="sxs-lookup"><span data-stu-id="61f62-125">These methods are optional.</span></span>

### <a name="access-token"></a><span data-ttu-id="61f62-126">アクセストークン</span><span class="sxs-lookup"><span data-stu-id="61f62-126">Access token</span></span>

<span data-ttu-id="61f62-127">`getAccessToken({'scopes': scopes[]}) : Promise<string>`メソッドを実装する必要があります。</span><span class="sxs-lookup"><span data-stu-id="61f62-127">You must implement the `getAccessToken({'scopes': scopes[]}) : Promise<string>` method.</span></span> <span data-ttu-id="61f62-128">このメソッドは、Microsoft Graph へのすべての呼び出しの前に有効なトークンを取得するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="61f62-128">This method is used to get a valid token before every call to Microsoft Graph.</span></span>

### <a name="graph"></a><span data-ttu-id="61f62-129">反転</span><span class="sxs-lookup"><span data-stu-id="61f62-129">Graph</span></span>

<span data-ttu-id="61f62-130">これらのコンポーネントは、microsoft graph のすべての呼び出しに Microsoft Graph Javascript SDK を使用します。</span><span class="sxs-lookup"><span data-stu-id="61f62-130">The components use the Microsoft Graph Javascript SDK for all calls to Microsoft Graph.</span></span> <span data-ttu-id="61f62-131">プロバイダーは、 `graph`プロパティで SDK を使用できるようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="61f62-131">Your provider must make the SDK available through the `graph` property.</span></span> <span data-ttu-id="61f62-132">のように、コンストラクターで新しい`Graph`インスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="61f62-132">In your constructor, create a new `Graph` instance, as shown.</span></span>

```js
this.graph = new Graph(this);
```

<span data-ttu-id="61f62-133">`Graph`クラスは、MICROSOFT Graph SDK の一番上にあるライトラッパーです。</span><span class="sxs-lookup"><span data-stu-id="61f62-133">The `Graph` class is a light wrapper on top of the Microsoft Graph SDK.</span></span>

### <a name="example"></a><span data-ttu-id="61f62-134">例</span><span class="sxs-lookup"><span data-stu-id="61f62-134">Example</span></span>

<span data-ttu-id="61f62-135">すべてのプロバイダーが抽象`IProvider`クラスを拡張します。</span><span class="sxs-lookup"><span data-stu-id="61f62-135">All the providers extend the `IProvider` abstract class.</span></span> <span data-ttu-id="61f62-136">例については、[既存のプロバイダー](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/src/providers)のソースコードを参照してください。</span><span class="sxs-lookup"><span data-stu-id="61f62-136">For examples, take a look at the source code for any of the [existing providers](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/src/providers).</span></span>

## <a name="set-the-global-provider"></a><span data-ttu-id="61f62-137">グローバルプロバイダーを設定する</span><span class="sxs-lookup"><span data-stu-id="61f62-137">Set the global provider</span></span>

<span data-ttu-id="61f62-138">コンポーネントは、 `Providers.globalProvider`プロパティを使用してプロバイダーにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="61f62-138">Components use the `Providers.globalProvider` property to access a provider.</span></span> <span data-ttu-id="61f62-139">独自のプロバイダーを作成した後、このプロパティをプロバイダーに設定します。</span><span class="sxs-lookup"><span data-stu-id="61f62-139">After you create your own provider, set this property to your provider.</span></span>

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

<span data-ttu-id="61f62-140">すべてのコンポーネントは新しいプロバイダーに通知され、その使用を開始します。</span><span class="sxs-lookup"><span data-stu-id="61f62-140">All the components will be notified of the new provider and start using it.</span></span>
