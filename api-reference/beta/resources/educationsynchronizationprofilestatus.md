---
title: educationSynchronizationProfileStatus リソースの種類
description: '学校のデータの同期プロファイルの同期の状態を表します。 '
author: mmast-msft
ms.openlocfilehash: c92ba2226b28896f8df89a7aee66602651344154
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325999"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>educationSynchronizationProfileStatus リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

学校のデータ[の同期プロファイル](educationsynchronizationprofile.md)の同期の状態を表します。 

> **注:****EducationSynchronizationProfileStatus**への更新はバック グラウンドで同期処理の非同期の性質のため遅れる可能性があります。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-|:-|:-|
| [同期のステータスを取得します。](../api/educationsynchronizationprofilestatus-get.md) | **educationSynchronizationProfileStatus** | 特定の同期プロファイルの状態を返します。 |

## <a name="properties"></a>Properties

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **status** | string | 同期の状態です。使用可能な値: `paused`、 `inProgress`、 `success`、 `error`、 `quarantined`、 `validationError`。 |
| **lastSynchronizationDateTime** | DateTimeOffset | ディレクトリ内の最新の変更が確認されて、時間を表します。  |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```