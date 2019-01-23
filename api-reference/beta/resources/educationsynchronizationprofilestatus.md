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
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="5def8-103">educationSynchronizationProfileStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5def8-103">educationSynchronizationProfileStatus resource type</span></span>

> <span data-ttu-id="5def8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5def8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5def8-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5def8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5def8-106">学校のデータ[の同期プロファイル](educationsynchronizationprofile.md)の同期の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="5def8-106">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="5def8-107">**注:\*\*\*\*EducationSynchronizationProfileStatus**への更新はバック グラウンドで同期処理の非同期の性質のため遅れる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5def8-107">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="5def8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5def8-108">Methods</span></span>

| <span data-ttu-id="5def8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5def8-109">Method</span></span> | <span data-ttu-id="5def8-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5def8-110">Return Type</span></span> | <span data-ttu-id="5def8-111">説明</span><span class="sxs-lookup"><span data-stu-id="5def8-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="5def8-112">同期のステータスを取得します。</span><span class="sxs-lookup"><span data-stu-id="5def8-112">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="5def8-113">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="5def8-113">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="5def8-114">特定の同期プロファイルの状態を返します。</span><span class="sxs-lookup"><span data-stu-id="5def8-114">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="5def8-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5def8-115">Properties</span></span>

| <span data-ttu-id="5def8-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5def8-116">Property</span></span> | <span data-ttu-id="5def8-117">型</span><span class="sxs-lookup"><span data-stu-id="5def8-117">Type</span></span> | <span data-ttu-id="5def8-118">説明</span><span class="sxs-lookup"><span data-stu-id="5def8-118">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="5def8-119">**status**</span><span class="sxs-lookup"><span data-stu-id="5def8-119">**status**</span></span> | <span data-ttu-id="5def8-120">educationSynchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="5def8-120">educationSynchronizationStatus</span></span> | <span data-ttu-id="5def8-121">同期の状態です。使用可能な値: `paused`、 `inProgress`、 `success`、 `error`、 `quarantined`、 `validationError`。</span><span class="sxs-lookup"><span data-stu-id="5def8-121">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="5def8-122">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="5def8-122">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="5def8-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5def8-123">DateTimeOffset</span></span> | <span data-ttu-id="5def8-124">ディレクトリ内の最新の変更が確認されて、時間を表します。</span><span class="sxs-lookup"><span data-stu-id="5def8-124">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="5def8-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5def8-125">JSON representation</span></span>
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
