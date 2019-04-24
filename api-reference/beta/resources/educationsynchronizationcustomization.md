---
title: educationSynchronizationCustomization リソースの種類
description: 'リソースエンティティの学校データプロファイルの同期をカスタマイズするための設定を提供します。 カスタマイズは、同期対象のすべてのエンティティに適用できます。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507050"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="4e4e4-104">educationSynchronizationCustomization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4e4e4-104">educationSynchronizationCustomization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e4e4-105">リソースエンティティの学校データプロファイルの同期をカスタマイズするための設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="4e4e4-105">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="4e4e4-106">カスタマイズは、同期対象のすべてのエンティティに適用できます。</span><span class="sxs-lookup"><span data-stu-id="4e4e4-106">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="4e4e4-107">**注:\*\*\*\*同期**開始プロパティは、 **StudentEnrollment**エンティティにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="4e4e4-107">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="4e4e4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e4e4-108">Properties</span></span>

| <span data-ttu-id="4e4e4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e4e4-109">Property</span></span> | <span data-ttu-id="4e4e4-110">型</span><span class="sxs-lookup"><span data-stu-id="4e4e4-110">Type</span></span> | <span data-ttu-id="4e4e4-111">説明</span><span class="sxs-lookup"><span data-stu-id="4e4e4-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="4e4e4-112">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="4e4e4-112">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="4e4e4-113">文字列のコレクション</span><span class="sxs-lookup"><span data-stu-id="4e4e4-113">collection of string</span></span> |  <span data-ttu-id="4e4e4-114">同期するプロパティ名のコレクション。null に設定されている場合、すべてのプロパティが同期されます。</span><span class="sxs-lookup"><span data-stu-id="4e4e4-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="4e4e4-115">**同期開始日**</span><span class="sxs-lookup"><span data-stu-id="4e4e4-115">**synchronizationStartDate**</span></span> | <span data-ttu-id="4e4e4-116">DateTime
</span><span class="sxs-lookup"><span data-stu-id="4e4e4-116">DateTime</span></span> |  <span data-ttu-id="4e4e4-117">同期を開始する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e4e4-117">The date that the synchronization should start.</span></span> <span data-ttu-id="4e4e4-118">この値は、将来の日付に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4e4e4-118">This value should be set to a future date.</span></span> <span data-ttu-id="4e4e4-119">null に設定されている場合、プロファイルの設定が完了すると、リソースが同期されます。</span><span class="sxs-lookup"><span data-stu-id="4e4e4-119">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="4e4e4-120">**注:** これは、 **StudentEnrollment**プロパティにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="4e4e4-120">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="4e4e4-121">**issyncdeferred**</span><span class="sxs-lookup"><span data-stu-id="4e4e4-121">**isSyncDeferred**</span></span> |<span data-ttu-id="4e4e4-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e4e4-122">Boolean</span></span> | <span data-ttu-id="4e4e4-123">親エンティティの同期を後日延期するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4e4e4-123">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="4e4e4-124">**allowdisplaynameupdate**</span><span class="sxs-lookup"><span data-stu-id="4e4e4-124">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="4e4e4-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e4e4-125">Boolean</span></span> |  <span data-ttu-id="4e4e4-126">同期によってリソースの表示名を上書きできるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4e4e4-126">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="4e4e4-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4e4e4-127">JSON representation</span></span>
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
