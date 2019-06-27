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
# <a name="login-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph ツールキットのログインコンポーネント

ログインコンポーネントは、Microsoft identity platform 認証を容易にするためのボタンとフライアウトのコントロールです。 2つの状態が提供されます。
* ユーザーがサインインしていない場合、コントロールは、サインインプロセスを開始するための簡単なボタンです。
* ユーザーがサインインしている場合、コントロールには現在サインインしているユーザー名、プロファイル画像、電子メールが表示されます。 このボタンをクリックすると、サインアウトするコマンドが表示されたフライアウトが開きます。

## <a name="example"></a>例

[jsfiddle の例](https://jsfiddle.net/metulev/scb9muh4)

```html
<mgt-login></mgt-login>
```

## <a name="using-the-control-without-an-authentication-provider"></a>認証プロバイダを使用しないコントロールの使用

このコンポーネントは、プロバイダーと、ボックスからの Microsoft Graph を使用して動作します。 ただし、独自のロジックと認証を提供する場合は、 `userDetails`プロパティを使用して、サインインしているユーザーの詳細を設定できます。 

| プロパティ | 属性 | 説明 |
| --- | --- | -- |
| `userDetails` | `user-details` | コントロールに表示されるユーザーオブジェクトを設定します。 |

次の例では、個人情報を設定します。

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    email: 'nikola@contoso.com',
    profileImage: 'url'
}
```

に`userDetails`設定`null`すると、サインアウト済みの状態に進みます。

`loginInitiated`および`logoutInitiated`イベントを使用して、サインインおよびサインインを処理します。 

## <a name="css-custom-properties"></a>CSS カスタムプロパティ

コンポーネント`mgt-login`は、次の CSS カスタムプロパティを定義します。

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

詳細については、「[スタイルコンポーネント](../style.md)」を参照してください。

## <a name="events"></a>イベント

コントロールから、次のイベントが発生します。

| イベント | 説明 |
| --- | --- |
| `loginInitiated` | ユーザーが [サインイン] ボタンをクリックして、ログイン処理を開始しました-キャンセル済み。|
| `loginCompleted` | ログインプロセスは正常に実行され、ユーザーはサインインしました。 |
| `loginFailed` | ユーザーがログインプロセスをキャンセルしたか、サインインできませんでした。|
| `logoutInitiated` | ユーザーが取り消しを開始しました。 |
| `logoutCompleted` | ユーザーがサインアウトした。 |

## <a name="microsoft-graph-permissions"></a>Microsoft Graph のアクセス許可

このコンポーネントは、 [Person コンポーネント](./person.md)を使用してユーザーを表示し、すべてのアクセス許可を継承します。 

## <a name="authentication"></a>認証

ログインコントロールは、[認証のドキュメント](./../providers.md)で説明されているグローバル認証プロバイダを使用します。 
