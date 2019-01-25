---
title: 設定の更新
description: '設定オブジェクトのプロパティを更新します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d21d7fb26945e4a46fdf877bb5911aba0621ce3b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508763"
---
# <a name="update-settings"></a>設定の更新

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[設定](../resources/user-settings.md)オブジェクトのプロパティを更新します。 同じ組織内のユーザーは、優先順位または組織のポリシーに基づいて、異なる設定を持つことができます。 ユーザーの現在の設定を取得、[現在のユーザー設定](user-get-settings.md)を参照してください。 

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | User.ReadWrite、User.ReadWrite.All   |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | User.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

```http
PATCH https://graph.microsoft.com/beta/me/settings
```

'UserPrincipalName' は、ユーザー、または User.ReadWrite.All のアクセス許可を持つユーザーがアクセス可能なや、ユーザー id が要求されます。 詳細については、[アクセス許可](/graph/permissions-reference)を参照してください。 

```http
PATCH https://graph.microsoft.com/beta/users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー       | 値|
|:-----------|:------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文

要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|ブール値|True を設定するには、 [Trending](../resources/insights-trending.md) API およびユーザーの Office についてのドキュメントへのアクセスを無効にする代理人へのアクセスは無効にします。 Office 365 に表示されるコンテンツの関連性に影響を与えるも true に設定 - 候補のサイトでは、SharePoint のホームとビジネスの OneDrive の検索ビューの関連性の低い結果を表示するたとえば、します。 この設定は、 [Office の説明](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)でコントロールの状態を反映しています。|

## <a name="example"></a>例 

##### <a name="request"></a>要求

Delve のユーザーを無効にし、組織全体のコンテンツの関連性に関する彼の貢献度を無効にする方法について、例の要求は、ここで。

```http
PATCH https://graph.microsoft.com/beta/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a>バッチ要求

Delve から複数のユーザーを無効にし、バッチ要求を組織全体でのコンテンツの関連性のような貢献を無効にすることもできます。
詳細については、 [JSON のバッチ処理](/graph/json-batching)を参照してください。

**重要**: だけで、[組織の管理](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US)役割グループのメンバーは、複数のユーザーを更新できます。 


<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-update-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
