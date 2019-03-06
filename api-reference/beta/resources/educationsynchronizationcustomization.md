---
title: educationSynchronizationCustomization リソースの種類
description: 'リソース エンティティの学校データ プロファイルの同期をカスタマイズするための設定を提供します。 同期されているすべてのエンティティには、カスタマイズを適用できます。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513607"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="64b72-104">educationSynchronizationCustomization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64b72-104">educationSynchronizationCustomization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64b72-105">リソース エンティティの学校データ プロファイルの同期をカスタマイズするための設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="64b72-105">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="64b72-106">同期されているすべてのエンティティには、カスタマイズを適用できます。</span><span class="sxs-lookup"><span data-stu-id="64b72-106">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="64b72-107">**注:** **SynchronizationStartDate**プロパティは、 **StudentEnrollment**のエンティティにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="64b72-107">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="64b72-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64b72-108">Properties</span></span>

| <span data-ttu-id="64b72-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64b72-109">Property</span></span> | <span data-ttu-id="64b72-110">型</span><span class="sxs-lookup"><span data-stu-id="64b72-110">Type</span></span> | <span data-ttu-id="64b72-111">説明</span><span class="sxs-lookup"><span data-stu-id="64b72-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="64b72-112">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="64b72-112">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="64b72-113">Collection of String</span><span class="sxs-lookup"><span data-stu-id="64b72-113">collection of string</span></span> |  <span data-ttu-id="64b72-114">同期するプロパティ名のコレクションです。かどうかのセットを null に、すべてのプロパティが同期します。</span><span class="sxs-lookup"><span data-stu-id="64b72-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="64b72-115">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="64b72-115">**synchronizationStartDate**</span></span> | <span data-ttu-id="64b72-116">DateTime
</span><span class="sxs-lookup"><span data-stu-id="64b72-116">DateTime</span></span> |  <span data-ttu-id="64b72-117">同期を開始する日付。</span><span class="sxs-lookup"><span data-stu-id="64b72-117">The date that the synchronization should start.</span></span> <span data-ttu-id="64b72-118">この値は、将来の日付に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="64b72-118">This value should be set to a future date.</span></span> <span data-ttu-id="64b72-119">場合は null の場合、リソースに設定は、プロファイルの設定が完了したときに同期されます。</span><span class="sxs-lookup"><span data-stu-id="64b72-119">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="64b72-120">**注:** これは、 **StudentEnrollment**プロパティにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="64b72-120">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="64b72-121">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="64b72-121">**isSyncDeferred**</span></span> |<span data-ttu-id="64b72-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="64b72-122">Boolean</span></span> | <span data-ttu-id="64b72-123">親エンティティの同期がそれ以降の日付に延期されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="64b72-123">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="64b72-124">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="64b72-124">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="64b72-125">ブール値</span><span class="sxs-lookup"><span data-stu-id="64b72-125">Boolean</span></span> |  <span data-ttu-id="64b72-126">同期によって、リソースの表示名を上書きするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="64b72-126">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="64b72-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64b72-127">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
