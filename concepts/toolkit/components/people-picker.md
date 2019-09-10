---
title: ユーザー選択コンポーネント
description: ユーザー選択ウィンドウを使用して、指定した数のユーザーを検索し、Microsoft Graph を使用して結果の一覧を表示することができます。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 2a0680a70ddfd5410e82911e5280c0b1a7e7dcaf
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822796"
---
# <a name="people-picker-component"></a>ユーザー選択コンポーネント

`mgt-people-picker` Web コンポーネント検索を使用して、指定した数のユーザーを検索し、結果の一覧を Microsoft Graph を介してレンダリングすることができます。 既定では、このコンポーネントはすべてのユーザーを検索します。また、グループのプロパティを定義して、結果をさらにフィルター処理することもできます。

表示する人の数がこの`show-max`値を超える場合、返されたすべてのユーザーが検索リストに表示されるわけではありません。

## <a name="example"></a>例

[jsfiddle の例](https://jsfiddle.net/metulev/jdv38fg0/)

```html
<mgt-people-picker></mgt-people-picker>
```

![「ユーザーの選択」](./images/mgt-people-picker-image.png)

## <a name="properties"></a>プロパティ

既定では、 `mgt-people-picker`コンポーネントは`/me/people`エンドポイントからイベントをフェッチします。 この動作を変更するには、次の属性を使用します。

| プロパティ | 属性 | 説明                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| showMax  | show-max  | 表示するユーザーの最大数を示す整数値。 既定値は6です。                                                                                             |
| people   | people    | コンポーネントによってレンダリングされたユーザーのリストを取得または設定するユーザーの配列。 このプロパティを使用して、コンポーネントによって読み込まれた人物にアクセスします。 自分のユーザーを読み込むには、この値を設定します。 |
| group    | group     | 検索結果をさらにフィルター処理するために、Microsoft Graph で定義されたグループに属する文字列型 (string) の値を指定します。                                                                            |

次に例を示します。

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="css-custom-properties"></a>CSS カスタムプロパティ

コンポーネント`mgt-people-picker`は、次の CSS カスタムプロパティを定義します。

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="microsoft-graph-permissions"></a>Microsoft Graph のアクセス許可

このコンポーネントは、次の Microsoft Graph Api とアクセス許可を使用します。

| API                                                                                                              | アクセス許可  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/ユーザー](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0)                    | People.Read |
| [/グループ/\${groupId}/メンバー](https://docs.microsoft.com/en-us/graph/api/group-list-members?view=graph-rest-1.0) | People.Read |

## <a name="authentication"></a>認証

このコントロールは、[認証のドキュメント](./../providers.md)で説明されているグローバル認証プロバイダを使用します。
