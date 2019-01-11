---
title: educationSynchronizationCustomization リソースの種類
description: 'リソース エンティティの学校データ プロファイルの同期をカスタマイズするための設定を提供します。 同期されているすべてのエンティティには、カスタマイズを適用できます。 '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 9294af5796daeefb394ed1625a9a36128ae7b2a4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860901"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="4f810-104">educationSynchronizationCustomization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4f810-104">educationSynchronizationCustomization resource type</span></span>

> <span data-ttu-id="4f810-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4f810-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f810-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f810-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4f810-107">リソース エンティティの学校データ プロファイルの同期をカスタマイズするための設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="4f810-107">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="4f810-108">同期されているすべてのエンティティには、カスタマイズを適用できます。</span><span class="sxs-lookup"><span data-stu-id="4f810-108">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="4f810-109">**注:\*\*\*\*SynchronizationStartDate**プロパティは、 **StudentEnrollment**のエンティティにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="4f810-109">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="4f810-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f810-110">Properties</span></span>

| <span data-ttu-id="4f810-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f810-111">Property</span></span> | <span data-ttu-id="4f810-112">種類</span><span class="sxs-lookup"><span data-stu-id="4f810-112">Type</span></span> | <span data-ttu-id="4f810-113">説明</span><span class="sxs-lookup"><span data-stu-id="4f810-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="4f810-114">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="4f810-114">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="4f810-115">文字列のコレクション</span><span class="sxs-lookup"><span data-stu-id="4f810-115">collection of string</span></span> |  <span data-ttu-id="4f810-116">同期するプロパティ名のコレクションです。かどうかのセットを null に、すべてのプロパティが同期します。</span><span class="sxs-lookup"><span data-stu-id="4f810-116">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="4f810-117">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="4f810-117">**synchronizationStartDate**</span></span> | <span data-ttu-id="4f810-118">DateTime</span><span class="sxs-lookup"><span data-stu-id="4f810-118">DateTime</span></span> |  <span data-ttu-id="4f810-119">同期を開始する日付。</span><span class="sxs-lookup"><span data-stu-id="4f810-119">The date that the synchronization should start.</span></span> <span data-ttu-id="4f810-120">この値は、将来の日付に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4f810-120">This value should be set to a future date.</span></span> <span data-ttu-id="4f810-121">場合は null の場合、リソースに設定は、プロファイルの設定が完了したときに同期されます。</span><span class="sxs-lookup"><span data-stu-id="4f810-121">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="4f810-122">**注:** これは、 **StudentEnrollment**プロパティにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="4f810-122">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="4f810-123">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="4f810-123">**isSyncDeferred**</span></span> |<span data-ttu-id="4f810-124">ブール型</span><span class="sxs-lookup"><span data-stu-id="4f810-124">Boolean</span></span> | <span data-ttu-id="4f810-125">親エンティティの同期がそれ以降の日付に延期されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4f810-125">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="4f810-126">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="4f810-126">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="4f810-127">ブール型</span><span class="sxs-lookup"><span data-stu-id="4f810-127">Boolean</span></span> |  <span data-ttu-id="4f810-128">同期によって、リソースの表示名を上書きするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4f810-128">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="4f810-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4f810-129">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
