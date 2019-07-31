---
title: educationSynchronizationProfileStatus リソースの種類
description: '学校データ同期プロファイルの同期の状態を表します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 827d54fbedbf9c6f386063d82fd00e8eddfe7296
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972336"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>educationSynchronizationProfileStatus リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

学校データ[同期プロファイル](educationsynchronizationprofile.md)の同期の状態を表します。 

> **注:****EducationSynchronizationProfileStatus**への更新は、バックグラウンド同期処理の非同期の性質により遅延する可能性があります。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-|:-|:-|
| [同期の状態を取得する](../api/educationsynchronizationprofilestatus-get.md) | **educationSynchronizationProfileStatus** | 特定の同期プロファイルの状態を返します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **status** | educationSynchronizationStatus | 同期の状態。可能な値は`paused`、 `inProgress`、 `success` `error` `quarantined`、、、 `validationError`、です。 |
| **Last同期日時** | DateTimeOffset | ディレクトリで最新の変更が確認された時刻を表します。  |

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
