---
title: educationSynchronizationCustomizations リソースの種類
description: 存在する場合は、同期と、カスタマイズするエンティティの一覧に含まれています。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e513e64afb1478ca7b5cc5d53f1964d16d9928b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523254"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="22a92-103">educationSynchronizationCustomizations リソースの種類</span><span class="sxs-lookup"><span data-stu-id="22a92-103">educationSynchronizationCustomizations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22a92-104">存在する場合は、同期を[カスタマイズ](educationsynchronizationcustomization.md)して、エンティティの一覧に含まれています。</span><span class="sxs-lookup"><span data-stu-id="22a92-104">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="22a92-105">**注:** 同期プロパティのカスタマイズは、 **studentEnrollment**と**teacherRoster**のエンティティには適用されません。</span><span class="sxs-lookup"><span data-stu-id="22a92-105">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="22a92-106">このリソースは、次のデータ プロバイダーのメンバーです。</span><span class="sxs-lookup"><span data-stu-id="22a92-106">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="22a92-107">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="22a92-107">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="22a92-108">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="22a92-108">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="22a92-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22a92-109">Properties</span></span>

| <span data-ttu-id="22a92-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22a92-110">Property</span></span> | <span data-ttu-id="22a92-111">型</span><span class="sxs-lookup"><span data-stu-id="22a92-111">Type</span></span> | <span data-ttu-id="22a92-112">説明</span><span class="sxs-lookup"><span data-stu-id="22a92-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="22a92-113">学校</span><span class="sxs-lookup"><span data-stu-id="22a92-113">**school**</span></span> | [<span data-ttu-id="22a92-114">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="22a92-114">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="22a92-115">学校のエンティティのカスタマイズです。</span><span class="sxs-lookup"><span data-stu-id="22a92-115">Customization for a school entity.</span></span>        |
| <span data-ttu-id="22a92-116">**section**</span><span class="sxs-lookup"><span data-stu-id="22a92-116">**section**</span></span> | [<span data-ttu-id="22a92-117">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="22a92-117">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="22a92-118">セクション エンティティをカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="22a92-118">Customization for a section entity.</span></span>         |
| <span data-ttu-id="22a92-119">**生徒**。</span><span class="sxs-lookup"><span data-stu-id="22a92-119">**student**</span></span> | [<span data-ttu-id="22a92-120">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="22a92-120">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="22a92-121">受講者用のエンティティのカスタマイズです。</span><span class="sxs-lookup"><span data-stu-id="22a92-121">Customization for a student entity.</span></span>         |
| <span data-ttu-id="22a92-122">teacher</span><span class="sxs-lookup"><span data-stu-id="22a92-122">**teacher**</span></span> | [<span data-ttu-id="22a92-123">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="22a92-123">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="22a92-124">先生のエンティティのカスタマイズです。</span><span class="sxs-lookup"><span data-stu-id="22a92-124">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="22a92-125">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="22a92-125">**studentEnrollment**</span></span> | [<span data-ttu-id="22a92-126">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="22a92-126">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="22a92-127">受講者の登録用にカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="22a92-127">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="22a92-128">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="22a92-128">**teacherRoster**</span></span> | [<span data-ttu-id="22a92-129">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="22a92-129">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="22a92-130">教師名簿をカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="22a92-130">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="22a92-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22a92-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "section": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "student": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacher": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "studentEnrollment": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacherRoster": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"}
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomizations.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
