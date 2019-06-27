---
title: Microsoft Graph ツールキットのログインコンポーネント
description: ログインコンポーネントは、Microsoft identity platform 認証を容易にするためのボタンとフライアウトのコントロールです。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e7c657b3b6c9772b2d7b7b8e64a57c9982f4caef
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243056"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="94627-103">Microsoft Graph ツールキットのログインコンポーネント</span><span class="sxs-lookup"><span data-stu-id="94627-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="94627-104">ログインコンポーネントは、Microsoft identity platform 認証を容易にするためのボタンとフライアウトのコントロールです。</span><span class="sxs-lookup"><span data-stu-id="94627-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="94627-105">2つの状態が提供されます。</span><span class="sxs-lookup"><span data-stu-id="94627-105">It provides two states:</span></span>
* <span data-ttu-id="94627-106">ユーザーがサインインしていない場合、コントロールは、サインインプロセスを開始するための簡単なボタンです。</span><span class="sxs-lookup"><span data-stu-id="94627-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="94627-107">ユーザーがサインインしている場合、コントロールには現在サインインしているユーザー名、プロファイル画像、電子メールが表示されます。</span><span class="sxs-lookup"><span data-stu-id="94627-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="94627-108">このボタンをクリックすると、サインアウトするコマンドが表示されたフライアウトが開きます。</span><span class="sxs-lookup"><span data-stu-id="94627-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="94627-109">例</span><span class="sxs-lookup"><span data-stu-id="94627-109">Example</span></span>

[<span data-ttu-id="94627-110">jsfiddle の例</span><span class="sxs-lookup"><span data-stu-id="94627-110">jsfiddle example</span></span>](https://jsfiddle.net/metulev/scb9muh4)

```html
<mgt-login></mgt-login>
```

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="94627-111">認証プロバイダを使用しないコントロールの使用</span><span class="sxs-lookup"><span data-stu-id="94627-111">Using the control without an authentication provider</span></span>

<span data-ttu-id="94627-112">このコンポーネントは、プロバイダーと、ボックスからの Microsoft Graph を使用して動作します。</span><span class="sxs-lookup"><span data-stu-id="94627-112">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="94627-113">ただし、独自のロジックと認証を提供する場合は、 `userDetails`プロパティを使用して、サインインしているユーザーの詳細を設定できます。</span><span class="sxs-lookup"><span data-stu-id="94627-113">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="94627-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94627-114">Property</span></span> | <span data-ttu-id="94627-115">属性</span><span class="sxs-lookup"><span data-stu-id="94627-115">Attribute</span></span> | <span data-ttu-id="94627-116">説明</span><span class="sxs-lookup"><span data-stu-id="94627-116">Description</span></span> |
| --- | --- | -- |
| `userDetails` | `user-details` | <span data-ttu-id="94627-117">コントロールに表示されるユーザーオブジェクトを設定します。</span><span class="sxs-lookup"><span data-stu-id="94627-117">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="94627-118">次の例では、個人情報を設定します。</span><span class="sxs-lookup"><span data-stu-id="94627-118">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    email: 'nikola@contoso.com',
    profileImage: 'url'
}
```

<span data-ttu-id="94627-119">に`userDetails`設定`null`すると、サインアウト済みの状態に進みます。</span><span class="sxs-lookup"><span data-stu-id="94627-119">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="94627-120">`loginInitiated`および`logoutInitiated`イベントを使用して、サインインおよびサインインを処理します。</span><span class="sxs-lookup"><span data-stu-id="94627-120">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="94627-121">CSS カスタムプロパティ</span><span class="sxs-lookup"><span data-stu-id="94627-121">CSS custom properties</span></span>

<span data-ttu-id="94627-122">コンポーネント`mgt-login`は、次の CSS カスタムプロパティを定義します。</span><span class="sxs-lookup"><span data-stu-id="94627-122">The `mgt-login` component defines the following CSS custom properties.</span></span>

```css
mgt-login {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --margin: 0;
  --padding: 12px 20px;
  --color: #201f1e;
  --background-color: transparent;
  --background-color--hover: #edebe9;
  --popup-content-background-color: white;
  --popup-command-font-size: 12px; }
}
```

<span data-ttu-id="94627-123">詳細については、「[スタイルコンポーネント](../style.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94627-123">To learn more, see [styling components](../style.md).</span></span>

## <a name="events"></a><span data-ttu-id="94627-124">イベント</span><span class="sxs-lookup"><span data-stu-id="94627-124">Events</span></span>

<span data-ttu-id="94627-125">コントロールから、次のイベントが発生します。</span><span class="sxs-lookup"><span data-stu-id="94627-125">The following events are fired from the control.</span></span>

| <span data-ttu-id="94627-126">イベント</span><span class="sxs-lookup"><span data-stu-id="94627-126">Event</span></span> | <span data-ttu-id="94627-127">説明</span><span class="sxs-lookup"><span data-stu-id="94627-127">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="94627-128">ユーザーが [サインイン] ボタンをクリックして、ログイン処理を開始しました-キャンセル済み。</span><span class="sxs-lookup"><span data-stu-id="94627-128">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="94627-129">ログインプロセスは正常に実行され、ユーザーはサインインしました。</span><span class="sxs-lookup"><span data-stu-id="94627-129">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="94627-130">ユーザーがログインプロセスをキャンセルしたか、サインインできませんでした。</span><span class="sxs-lookup"><span data-stu-id="94627-130">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="94627-131">ユーザーが取り消しを開始しました。</span><span class="sxs-lookup"><span data-stu-id="94627-131">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="94627-132">ユーザーがサインアウトした。</span><span class="sxs-lookup"><span data-stu-id="94627-132">The user signed out.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="94627-133">Microsoft Graph のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="94627-133">Microsoft Graph permissions</span></span>

<span data-ttu-id="94627-134">このコンポーネントは、 [Person コンポーネント](./person.md)を使用してユーザーを表示し、すべてのアクセス許可を継承します。</span><span class="sxs-lookup"><span data-stu-id="94627-134">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="94627-135">認証</span><span class="sxs-lookup"><span data-stu-id="94627-135">Authentication</span></span>

<span data-ttu-id="94627-136">ログインコントロールは、[認証のドキュメント](./../providers.md)で説明されているグローバル認証プロバイダを使用します。</span><span class="sxs-lookup"><span data-stu-id="94627-136">The login control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 
