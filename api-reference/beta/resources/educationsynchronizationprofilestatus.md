---
title: educationSynchronizationProfileStatus リソースの種類
description: '学校データ同期プロファイルの同期の状態を表します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 12908f6454cb27c673935f1e4c64c921b7ff0dcd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507092"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="ef81b-103">educationSynchronizationProfileStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef81b-103">educationSynchronizationProfileStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef81b-104">学校データ[同期プロファイル](educationsynchronizationprofile.md)の同期の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="ef81b-104">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="ef81b-105">**注:\*\*\*\*educationSynchronizationProfileStatus**への更新は、バックグラウンド同期処理の非同期の性質により遅延する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ef81b-105">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="ef81b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef81b-106">Methods</span></span>

| <span data-ttu-id="ef81b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef81b-107">Method</span></span> | <span data-ttu-id="ef81b-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ef81b-108">Return Type</span></span> | <span data-ttu-id="ef81b-109">説明</span><span class="sxs-lookup"><span data-stu-id="ef81b-109">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="ef81b-110">同期の状態を取得する</span><span class="sxs-lookup"><span data-stu-id="ef81b-110">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="ef81b-111">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="ef81b-111">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="ef81b-112">特定の同期プロファイルの状態を返します。</span><span class="sxs-lookup"><span data-stu-id="ef81b-112">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="ef81b-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef81b-113">Properties</span></span>

| <span data-ttu-id="ef81b-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef81b-114">Property</span></span> | <span data-ttu-id="ef81b-115">型</span><span class="sxs-lookup"><span data-stu-id="ef81b-115">Type</span></span> | <span data-ttu-id="ef81b-116">説明</span><span class="sxs-lookup"><span data-stu-id="ef81b-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ef81b-117">**status**</span><span class="sxs-lookup"><span data-stu-id="ef81b-117">**status**</span></span> | <span data-ttu-id="ef81b-118">educationSynchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="ef81b-118">educationSynchronizationStatus</span></span> | <span data-ttu-id="ef81b-119">同期の状態。可能な値は`paused`、 `inProgress`、 `success` `error` `quarantined`、、、 `validationError`、です。</span><span class="sxs-lookup"><span data-stu-id="ef81b-119">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="ef81b-120">**last同期日時**</span><span class="sxs-lookup"><span data-stu-id="ef81b-120">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="ef81b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef81b-121">DateTimeOffset</span></span> | <span data-ttu-id="ef81b-122">ディレクトリで最新の変更が確認された時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="ef81b-122">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="ef81b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ef81b-123">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationprofilestatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
