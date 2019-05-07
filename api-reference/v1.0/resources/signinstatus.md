---
title: signInStatus リソースの種類
description: サインインの状態 (成功または失敗) を提供します。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3a57e5bb0e53f5deec4d0c6d92541f7d2bd4744d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629223"
---
# <a name="signinstatus-resource-type"></a>signInStatus リソースの種類

サインインの状態 (成功または失敗) を提供します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|additionalDetails|String|サインインアクティビティについての追加情報を提供します。|
|errorCode|Int32|サインイン失敗時に生成される5桁のエラーコードを提供します。 [エラーコードとメッセージの一覧](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)を確認します。|
|failureReason|String|対応するサインインアクティビティのエラーメッセージまたはエラーの理由を示します。 [エラーコードとメッセージの一覧](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)を確認します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInStatus"
}-->

```json
{
  "additionalDetails": "String",
  "errorCode": 1024,
  "failureReason": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
