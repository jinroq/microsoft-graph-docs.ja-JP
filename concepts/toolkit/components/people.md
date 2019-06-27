---
title: Microsoft Graph ツールキットの People コンポーネント
description: '`mgt-people` Web コンポーネントを使用して、ユーザーまたは連絡先のグループを写真またはイニシャルを使用して表示できます。'
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: fcc44262f807d3f10f42e8af8e476975ad262cda
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243062"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph ツールキットの People コンポーネント

`mgt-people` Web コンポーネントを使用して、ユーザーまたは連絡先のグループを写真またはイニシャルを使用して表示できます。 既定では、サインインしているユーザーの最もよく使用される連絡先が表示されます。

このコンポーネントは複数の管理[者](./person.md)を使用していますが、一連のユーザー記述子にバインドできます。 表示するユーザー数がこの`show-max`値を超える場合は、追加の連絡先の数を示す番号が追加されます。

## <a name="example"></a>例

[jsfiddle の例](https://jsfiddle.net/metulev/az6pqy2r/)

```html
<mgt-people></mgt-people>
```

![「ユーザー」](./images/mgt-people.png)

## <a name="properties"></a>プロパティ

既定では、 `mgt-people`コンポーネントは、頻繁に`/me/people`接続され`personType/class eq 'Person'`たユーザーを表示するために、フィルターを使用してエンドポイントからイベントをフェッチします。 この動作を変更するには、いくつかのプロパティを使用できます。

| プロパティ | 属性 | 説明 |
| --- | --- | --- |
| `showMax` | `show-max` | 表示するユーザーの最大数を指定します。 既定値は3です。 |
| `people` | `people` | コンポーネントによってレンダリングされたユーザーのリストを取得または設定するユーザーの配列。 このプロパティを使用して、コンポーネントによって読み込まれた人物にアクセスします。 自分のユーザーを読み込むには、この値を設定します。 |

次の例では、表示するユーザーの最大数を設定します。

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a>CSS カスタムプロパティ

コンポーネント`mgt-people`は、次の CSS カスタムプロパティを定義します。

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a>テンプレート

は`mgt-people` 、コンポーネントの特定の部分を置き換えるために使用できるいくつかの[テンプレート](../templates.md)をサポートしています。 テンプレートを指定するには、 `<template>`コンポーネント内に要素を含め、 `data-type`値を次のいずれかに設定します。

| データ型 | データコンテキスト | 説明 |
| --- | --- | --- |
| `default` | `people`: person オブジェクトのリスト | 既定のテンプレートでは、コンポーネント全体が独自のものに置き換えられます。 |
| `person` | `person`: person オブジェクト | 各ユーザーのレンダリングに使用するテンプレート。 |
| `overflow` | `people`: person オブジェクトのリスト <br> `max`: 表示されているユーザーの数 <br> `extra`: 特別なユーザーの数 | ユーザーの一覧の右側に最大数を超える番号をレンダリングするために使用されるテンプレート。 |
| `no-data` | データコンテキストが渡されない | ユーザーが使用できない場合に使用するテンプレート。 |

次の例は、テンプレートの`person`使用方法を示しています。

```html
<mgt-people>
  <template>
    <ul><li data-for="person in people">
      <mgt-person person-query="{{ person.userPrincipalName }}"></mgt-person>
      <h3>{{ person.displayName }}</h3>
      <p>{{ person.jobTitle }}</p>
      <p>{{ person.department }}</p>
    </li></ul>
  </template>
</mgt-people>
```

## <a name="microsoft-graph-permissions"></a>Microsoft Graph のアクセス許可

このコンポーネントは、次の Microsoft Graph Api とアクセス許可を使用します。

| リソース | アクセス許可/スコープ |
| - | - |
| [/me/ユーザー](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |

## <a name="authentication"></a>認証

このコントロールは、[認証のドキュメント](./../providers.md)で説明されているグローバル認証プロバイダを使用します。
