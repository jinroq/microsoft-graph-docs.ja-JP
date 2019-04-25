---
title: 会社のリソースの種類
description: Dynamics 365 Business Central の会社。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: f1faca36af25bc8cb3e9019e0dc5b4460991e70d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543109"
---
# <a name="companies-resource-type"></a>会社のリソースの種類
Dynamics 365 Business Central の会社のリソースの種類を表します。 

## <a name="methods"></a>メソッド

| メソッド         | 戻り値の型  |説明|
|:---------------|:-------------|:----------|
|[会社名を取得する](../api/dynamics-companies-get.md)|companies|会社を取得します。|

## <a name="properties"></a>プロパティ
| プロパティ        | 型 |説明                             |
|:----------------|:-----|:---------------------------------------|
|id               |GUID  |会社の一意の ID。 読み取り専用です。|
|name             |string|会社を指定します。                  |
|displayName      |string|会社の表示名を指定します。     |
|systemversion    |string|会社の内部バージョンを指定します。|
|businessProfileId|string|会社にリンクされているビジネスプロファイル ID を指定します。|


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

以下は、会社の JSON 表記です。

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}

```


