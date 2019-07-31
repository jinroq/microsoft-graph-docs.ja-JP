---
title: educationSynchronizationCustomization リソースの種類
description: 'リソースエンティティの学校データプロファイルの同期をカスタマイズするための設定を提供します。 カスタマイズは、同期対象のすべてのエンティティに適用できます。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 46cd20bbe016110a313d5b195a518ef81ca05afe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972454"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="56e62-104">educationSynchronizationCustomization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="56e62-104">educationSynchronizationCustomization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56e62-105">リソースエンティティの学校データプロファイルの同期をカスタマイズするための設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="56e62-105">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="56e62-106">カスタマイズは、同期対象のすべてのエンティティに適用できます。</span><span class="sxs-lookup"><span data-stu-id="56e62-106">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="56e62-107">**注:\*\*\*\*同期**開始プロパティは、 **StudentEnrollment**エンティティにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="56e62-107">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="56e62-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56e62-108">Properties</span></span>

| <span data-ttu-id="56e62-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56e62-109">Property</span></span> | <span data-ttu-id="56e62-110">型</span><span class="sxs-lookup"><span data-stu-id="56e62-110">Type</span></span> | <span data-ttu-id="56e62-111">説明</span><span class="sxs-lookup"><span data-stu-id="56e62-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="56e62-112">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="56e62-112">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="56e62-113">文字列のコレクション</span><span class="sxs-lookup"><span data-stu-id="56e62-113">collection of string</span></span> |  <span data-ttu-id="56e62-114">同期するプロパティ名のコレクション。Null に設定されている場合、すべてのプロパティが同期されます。</span><span class="sxs-lookup"><span data-stu-id="56e62-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="56e62-115">**同期開始日**</span><span class="sxs-lookup"><span data-stu-id="56e62-115">**synchronizationStartDate**</span></span> | <span data-ttu-id="56e62-116">DateTime</span><span class="sxs-lookup"><span data-stu-id="56e62-116">DateTime</span></span> |  <span data-ttu-id="56e62-117">同期を開始する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="56e62-117">The date that the synchronization should start.</span></span> <span data-ttu-id="56e62-118">この値は、将来の日付に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="56e62-118">This value should be set to a future date.</span></span> <span data-ttu-id="56e62-119">Null に設定されている場合、プロファイルの設定が完了すると、リソースが同期されます。</span><span class="sxs-lookup"><span data-stu-id="56e62-119">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="56e62-120">**注:** これは、 **StudentEnrollment**プロパティにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="56e62-120">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="56e62-121">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="56e62-121">**isSyncDeferred**</span></span> |<span data-ttu-id="56e62-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="56e62-122">Boolean</span></span> | <span data-ttu-id="56e62-123">親エンティティの同期を後日延期するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="56e62-123">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="56e62-124">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="56e62-124">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="56e62-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="56e62-125">Boolean</span></span> |  <span data-ttu-id="56e62-126">同期によってリソースの表示名を上書きできるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="56e62-126">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="56e62-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="56e62-127">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
