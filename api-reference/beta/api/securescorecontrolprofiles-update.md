---
title: secureScoreControlProfiles の更新
description: 任意の統合ソリューション内の編集可能な securescorecontrolprofiles のプロパティを更新して、担当者または tenantnote などのさまざまなプロパティを変更します。
localization_priority: Normal
ms.openlocfilehash: ee184e921301fc8e2ce9e86122e5f01c335fa540
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331505"
---
# <a name="update-securescorecontrolprofiles"></a>secureScoreControlProfiles の更新

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

任意の統合ソリューション内の編集可能な**securescorecontrolprofiles の**プロパティを更新して、**担当者**または**tenantnote**などのさまざまなプロパティを変更します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |   securityevents。  |
|委任 (個人用 Microsoft アカウント) |  サポートされていません。  |
|アプリケーション | securityevents。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 説明|
|:-----------|:-----------|
| Authorization  | ベアラー {code}。 必須。|
|Prefer | 戻り値 = 表現。 |

## <a name="request-body"></a>要求本文

要求本文で、更新する必要のある関連フィールドの値の JSON 表記を指定します。 次の表に、secureScoreControlProfile で更新できるフィールドを示します。 要求本文に含まれていない既存のプロパティの値は変更されません。 最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|assignedTo|String|トリアージ、実装、または修復のために、コントロールが割り当てられているアナリストの名前。|
|tenantnote|String|コントロールに関するアナリストコメント (カスタマーコントロール管理向け)。|
|controlstateupdates| String|コントロールに対するアナリスト主導の設定。 可能な値は、`ignore`、`thirdParty`、`reviewed` です。|


## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

オプションの要求ヘッダーが使用されている場合、 `200 OK`メソッドは応答コードと、応答本文で更新された[securescorecontrolprofiles の](../resources/securescorecontrolprofiles.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "controlStateUpdates": "controlStateUpdates-value"
}
```

### <a name="response"></a>応答

成功応答の例を次に示します。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 204 No Content
```




<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
