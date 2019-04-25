---
title: 設定を更新する
description: 'settings オブジェクトのプロパティを更新します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eb739ebe4266dc61246fd39f1b4f053ab08a5a75
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573572"
---
# <a name="update-settings"></a>設定を更新する

[settings](../resources/user-settings.md)オブジェクトのプロパティを更新します。 同じ組織内のユーザーは、そのユーザーの好みまたは組織のポリシーに基づいて設定を変えることができます。 ユーザーの現在の設定を取得するには、「[現在のユーザーの設定](user-get-settings.md)」を参照してください。 

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | ユーザー読み取り/書き込みユーザー。   |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | User.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

```http
PATCH /me/settings
```

' user id ' または ' userPrincipalName ' を持つ要求は、ユーザーまたはすべてのアクセス許可を持つユーザーのみがアクセスできます。 詳細については、「 [Permissions](/graph/permissions-reference)」を参照してください。 

```http
PATCH /users/{id | userPrincipalName}/settings/
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
|contributionToContentDiscoveryDisabled|Boolean|true に設定[トレンド分析](/graph/api/resources/insights-trending?view=graph-rest-beta)API への代理人アクセスを無効にし、ユーザーの Office Delve でドキュメントへのアクセスを無効にします。 true に設定すると、Office 365 に表示されるコンテンツの関連性にも影響します。たとえば、SharePoint ホームのおすすめサイト、OneDrive for business の検出ビューには関連性の低い検索結果が表示されます。 この設定は、 [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)のコントロールの状態を反映します。|

## <a name="example"></a>例 

##### <a name="request"></a>要求

次に、Delve からユーザーをオプトアウトして、組織全体のコンテンツの関連性に関する投稿を無効にする方法についての要求の例を示します。

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
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

また、Delve から複数のユーザーをオプトアウトし、バッチ要求によって組織全体のコンテンツ関連性に対する貢献を無効にすることもできます。
詳細については、「 [JSON のバッチ](https://developer.microsoft.com/graph/docs/concepts/json_batching)処理」を参照してください。

**重要**:[組織の管理](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US)役割グループのメンバーのみが複数のユーザーを更新できます。 



