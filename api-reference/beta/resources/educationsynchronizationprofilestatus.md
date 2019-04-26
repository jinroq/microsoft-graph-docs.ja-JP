---
title: educationSynchronizationProfileStatus リソースの種類
description: '学校データ同期プロファイルの同期の状態を表します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e54a80df832eba66dcdc5eb08b38feee6f4cd57a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340496"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>educationSynchronizationProfileStatus リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

学校データ[同期プロファイル](educationsynchronizationprofile.md)の同期の状態を表します。 

> **注:****educationSynchronizationProfileStatus**への更新は、バックグラウンド同期処理の非同期の性質により遅延する可能性があります。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-|:-|:-|
| [同期の状態を取得する](../api/educationsynchronizationprofilestatus-get.md) | **educationSynchronizationProfileStatus** | 特定の同期プロファイルの状態を返します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **status** | educationSynchronizationStatus | 同期の状態。可能な値は`paused`、 `inProgress`、 `success` `error` `quarantined`、、、 `validationError`、です。 |
| **last同期日時** | DateTimeOffset | ディレクトリで最新の変更が確認された時刻を表します。  |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```
