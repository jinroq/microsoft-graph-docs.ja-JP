---
title: educationSynchronizationProfileStatus リソースの種類
description: '学校のデータの同期プロファイルの同期の状態を表します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1fd77f48544e5e6bc0c582e4ce9fb2a5b1b6601a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396155"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>educationSynchronizationProfileStatus リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

学校のデータ[の同期プロファイル](educationsynchronizationprofile.md)の同期の状態を表します。 

> **注:****EducationSynchronizationProfileStatus**への更新はバック グラウンドで同期処理の非同期の性質のため遅れる可能性があります。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-|:-|:-|
| [同期のステータスを取得します。](../api/educationsynchronizationprofilestatus-get.md) | **educationSynchronizationProfileStatus** | 特定の同期プロファイルの状態を返します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **status** | educationSynchronizationStatus | 同期の状態です。使用可能な値: `paused`、 `inProgress`、 `success`、 `error`、 `quarantined`、 `validationError`。 |
| **lastSynchronizationDateTime** | DateTimeOffset | ディレクトリ内の最新の変更が確認されて、時間を表します。  |

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
