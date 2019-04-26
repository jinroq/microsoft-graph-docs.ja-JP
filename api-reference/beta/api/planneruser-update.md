---
title: プランのユーザーを更新する
description: プランのユーザーオブジェクトのプロパティを更新します。 この操作を使用して、ユーザーのお気に入りのプランの一覧からプランを追加または削除したり、ユーザーが最近表示したプランを示したりすることができます。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 77f76a8b2324fd287cc3f73d1aa78a99accb4ea2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337559"
---
# <a name="update-planneruser"></a>プランのユーザーを更新する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[プランのユーザー](../resources/planneruser.md)オブジェクトのプロパティを更新します。 この操作を使用して、ユーザーのお気に入りのプランの一覧からプランを追加または削除したり、ユーザーが最近表示したプランを示したりすることができます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Group.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a>オプションの要求ヘッダー
| 名前       | 説明|
|:-----------|:-----------|
| Authorization  | ベアラー {code}。 必須です。|
| If-Match  | 更新する**プラン**の最後の既知の ETag 値。 必須です。|

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。 要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。 最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|お気に入りプランの参照|[plannerFavoritePlanReferenceCollection](../resources/plannerfavoriteplanreferencecollection.md)|ユーザーがお気に入りとしてマークしたプランへの参照が含まれているコレクションに対する変更。|
|recentPlanReferences|[plannerRecentPlanReferenceCollection](../resources/plannerrecentplanreferencecollection.md)|ユーザーが最近表示したプランへの参照が含まれているコレクションに対する変更。|

## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[プランのユーザー](../resources/planneruser.md)オブジェクトを返します。

このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。
## <a name="example"></a>例
##### <a name="request"></a>要求
要求の例を次に示します。 この要求は、"jd8S5gOaFk2S8aWCIAJz42QAAxtD" という id を持つプラン "次のリリースディスカッション" をユーザーのお気に入りとして追加し、"7oTB5aMIAE2rVo-1n-L7RmQAGX2q" という id のプランを [お気に入りのプラン] の一覧から削除します。
また、"jd8S5gOaFk2S8aWCIAJz42QAAxtD" プランの最終ビュー時刻も更新します。
<!-- {
  "blockType": "ignored",
  "name": "update_planneruser"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/planner
Content-type: application/json
Content-length: 504
If-Match: W/"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc="

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": " !",
      "planTitle": "Next Release Discussion"
    },
    "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": null
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    }
  }
}
```
##### <a name="response"></a>応答
応答の例を次に示します。 

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586866870001551087",
      "planTitle": "Next Release Discussion"
    },
    "uZWtCtli30CGoWLIWSat1mQAC0ai": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586888705198093378",
      "planTitle": "Product Support"
    }
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    },
    "XYE5pqNJu0uuRC2PM4ZQrmQAF2Pn": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-01T19:39:17.57Z",
      "planTitle": "Success Metrics"
    }
  },
  "id": "-YPnMJRiIUSKFyaVjYEkBWQAAc47"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update planneruser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
