---
title: appliedConditionalAccessPolicy リソースの種類
description: 適用される条件付きアクセスポリシーに関連する属性を示します。このポリシーは、対応するサインインアクティビティによってトリガーされます。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bb5562b07e60b10a36dafac37d5839d9bacc060a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629342"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>appliedConditionalAccessPolicy リソースの種類

適用される条件付きアクセスポリシーに関連する属性を示します。このポリシーは、対応するサインインアクティビティによってトリガーされます。

## <a name="properties"></a>プロパティ

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|displayName|String|条件付きアクセスポリシーの名前を参照します (例: "Salesforce の MFA が必要")。|
|enforcedGrantControls|String collection|条件付きアクセスポリシーによって適用される grant コントロールを参照します (例: "多要素認証を必要とする")。|
|enforcedSessionControls|String collection|条件付きアクセスポリシーによって適用されるセッションコントロールを参照します (例: "アプリ強制コントロールが必要です")。|
|id|文字列|条件付きアクセスの一意の GUID。 y|
|result|String| トリガーされた CA ポリシーの結果を示します。 使用可能な値は次のいずれかです。<br/>`success`<br/>`failure`<br/>`notApplied`-ポリシー条件が満たされていないため、ポリシーは適用されません。<br/>`notEnabled`-これは、ポリシーが無効な状態になっているためです。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
}-->

```json
{
  "displayName": "String",
  "enforcedGrantControls": ["String"],
  "enforcedSessionControls": ["String"],
  "id": "String",
  "result": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appliedConditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
