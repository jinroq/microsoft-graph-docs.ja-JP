---
title: Microsoft Graph ツールキットの Person コンポーネント
description: Person コンポーネントは、ユーザーまたは連絡先を、自分の写真、名前、電子メールアドレスを使用して表示するために使用されます。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b9102259258bb691dee2c56449257740db7b1913
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243038"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph ツールキットの Person コンポーネント

Person コンポーネントは、ユーザーまたは連絡先を、自分の写真、名前、電子メールアドレスを使用して表示するために使用されます。 

## <a name="example"></a>例

[jsfiddle の例](https://jsfiddle.net/metulev/0jkzfr42/)

### <a name="add-the-control-to-the-html-page"></a>HTML ページにコントロールを追加する
```html
<mgt-person person-query=""></mgt-person>
```

## <a name="setting-the-person-details"></a>個人情報の設定

3つのプロパティを使用して、人物の詳細を設定できます。 インスタンスごとに、次のいずれかのプロパティを使用します。

* `user-id`属性または`userId`プロパティを設定して、ID を使用して Microsoft Graph からユーザーを取得します。  

* 特定の`person-query`ユーザーの`personQuery` Microsoft Graph を検索するように、属性またはプロパティを設定します。 最初に使用可能な人物を選択し、ユーザーの詳細を取得します。 電子メールは、適切な人物に対してクエリを実行することをお勧めしますが、名前も同じように動作します。

* 次の`person-details`例に`personDetails`示すように、手動で個人情報を設定するように属性またはプロパティを設定します。


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  イメージが指定されていない場合は、取得されます (使用可能な場合)。

## <a name="changing-how-the-component-looks"></a>コンポーネントの外観の変更

複数のプロパティを使用して、コンポーネントをカスタマイズできます。

| プロパティ | 属性 | 説明 |
| --- | --- | --- |
| `showName` | `show-name` | ユーザーの表示名を表示するフラグを設定`false`します。既定値はです。 |
| `showEmail` | `show-email` | ユーザーの電子メールを表示するフラグを`false`設定します。既定値はです。 |

## <a name="css-custom-properties"></a>CSS カスタムプロパティ

コンポーネント`mgt-person`は、次の CSS カスタムプロパティを定義します。

```css
mgt-person {
  --avatar-size-s: 24px;
  --avatar-size: 48px; // avatar size when both name and email are shown
  --avatar-font-size--s: 16px;
  --avatar-font-size: 32px; // font-size when both name and email are shown
  --avatar-border: 0;
  --initials-color: white;
  --initials-background-color: magenta;
  --font-size: 12px;
  --font-weight: 500;
  --color: black;
  --email-font-size: 12px;
  --email-color: black;
}
```

詳細については、「[スタイルコンポーネント](../style.md)」を参照してください。

## <a name="templates"></a>テンプレート

コンポーネント`mgt-person`は、コンポーネントの特定の部分を置き換えることができるいくつかの[テンプレート](../templates.md)をサポートしています。 テンプレートを指定するには、 `<template>`コンポーネント内に要素を含め、 `data-type`値を次のいずれかに設定します。

| データ型 | データコンテキスト | 説明 |
| --- | --- | --- |
| `default` | `person`: person オブジェクト | 既定のテンプレートでは、コンポーネント全体が独自のものに置き換えられます。 |

次の例では、person コンポーネントのテンプレートを定義します。

```html
<mgt-person>
  <template>
    <div data-if="person.image">
      <img src="{{person.image}}" />
    </div>
    <div data-else>
      {{person.displayName}}
    </div>
  </template>
</mgt-person>
```

## <a name="microsoft-graph-permissions"></a>Microsoft Graph のアクセス許可

このコントロールでは、次の Microsoft Graph Api とアクセス許可を使用します。

| リソース | アクセス許可/スコープ |
| - | - |
| [/me](https://docs.microsoft.com/en-us/graph/api/user-get?view=graph-rest-1.0) | `User.Read` |
| [/me¥ photo/$value](https://docs.microsoft.com/en-us/graph/api/profilephoto-get?view=graph-rest-beta) | `User.Read` |
| [/me/people/? $search =](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |
| [/me/contacts/*](https://docs.microsoft.com/en-us/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | `Contacts.Read` |
| [/ユーザー/_/_/_/$value](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `User.ReadBasic.All` |

> **注:** 個人用の`*/photo/$value` microsoft アカウントのリソースにアクセスするには、microsoft Graph ベータ版エンドポイントを使用します。

## <a name="authentication"></a>認証

このコントロールは、[認証のドキュメント](./../providers.md)で説明されているグローバル認証プロバイダを使用して、必要なデータをフェッチします。
