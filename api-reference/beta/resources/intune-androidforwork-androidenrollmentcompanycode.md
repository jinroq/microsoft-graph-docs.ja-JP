---
title: androidEnrollmentCompanyCode リソースの種類
description: トークン、Url、QR コードコンテンツなど、Google の Android 管理 API 経由の登録に使用される、専門分野の登録データを保持するクラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ccc8cd1c1753c844ac5a71f9248f8189dad1e0b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367100"
---
# <a name="androidenrollmentcompanycode-resource-type"></a>androidEnrollmentCompanyCode リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

トークン、Url、QR コードコンテンツなど、Google の Android 管理 API 経由の登録に使用される、専門分野の登録データを保持するクラス

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|enrollmentToken|String|ユーザーがデバイスを登録するために使用する登録トークン。|
|qrCodeContent|String|トークンの QR コードを生成するために使用する文字列。|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|トークンの生成された QR コード。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```



