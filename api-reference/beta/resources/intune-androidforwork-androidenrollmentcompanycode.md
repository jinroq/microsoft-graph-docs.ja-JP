---
title: androidEnrollmentCompanyCode リソースの種類
description: トークン、Url、QR コードコンテンツなど、Google の Android 管理 API 経由の登録に使用される、専門分野の登録データを保持するクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0422bf09d990c02c984b45fa144d6ae12661f718
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784440"
---
# <a name="androidenrollmentcompanycode-resource-type"></a>androidEnrollmentCompanyCode リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

トークン、Url、QR コードコンテンツなど、Google の Android 管理 API 経由の登録に使用される、専門分野の登録データを保持するクラス

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|enrollmentToken|文字列|ユーザーがデバイスを登録するために使用する登録トークン。|
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





