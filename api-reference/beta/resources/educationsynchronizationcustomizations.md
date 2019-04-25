---
title: educationSynchronizationCustomizations リソースの種類
description: 同期するエンティティのリストと、そのカスタマイズがあればそれを含みます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e513e64afb1478ca7b5cc5d53f1964d16d9928b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543204"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="c70e1-103">educationSynchronizationCustomizations リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c70e1-103">educationSynchronizationCustomizations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c70e1-104">同期するエンティティのリストと、その[カスタマイズ](educationsynchronizationcustomization.md)があればそれを含みます。</span><span class="sxs-lookup"><span data-stu-id="c70e1-104">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="c70e1-105">**注:** 同期するプロパティのカスタマイズは、 **studentEnrollment**エンティティおよび**teacherRoster**エンティティには適用されません。</span><span class="sxs-lookup"><span data-stu-id="c70e1-105">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="c70e1-106">このリソースは、次のデータプロバイダーのメンバーです。</span><span class="sxs-lookup"><span data-stu-id="c70e1-106">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="c70e1-107">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="c70e1-107">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="c70e1-108">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="c70e1-108">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="c70e1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c70e1-109">Properties</span></span>

| <span data-ttu-id="c70e1-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c70e1-110">Property</span></span> | <span data-ttu-id="c70e1-111">型</span><span class="sxs-lookup"><span data-stu-id="c70e1-111">Type</span></span> | <span data-ttu-id="c70e1-112">説明</span><span class="sxs-lookup"><span data-stu-id="c70e1-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c70e1-113">**筆記**</span><span class="sxs-lookup"><span data-stu-id="c70e1-113">**school**</span></span> | [<span data-ttu-id="c70e1-114">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c70e1-114">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c70e1-115">学校エンティティのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="c70e1-115">Customization for a school entity.</span></span>        |
| <span data-ttu-id="c70e1-116">**セクション**</span><span class="sxs-lookup"><span data-stu-id="c70e1-116">**section**</span></span> | [<span data-ttu-id="c70e1-117">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c70e1-117">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c70e1-118">セクションエンティティのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="c70e1-118">Customization for a section entity.</span></span>         |
| <span data-ttu-id="c70e1-119">**学生**</span><span class="sxs-lookup"><span data-stu-id="c70e1-119">**student**</span></span> | [<span data-ttu-id="c70e1-120">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c70e1-120">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c70e1-121">学生エンティティのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="c70e1-121">Customization for a student entity.</span></span>         |
| <span data-ttu-id="c70e1-122">**teacher**</span><span class="sxs-lookup"><span data-stu-id="c70e1-122">**teacher**</span></span> | [<span data-ttu-id="c70e1-123">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c70e1-123">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c70e1-124">教師エンティティのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="c70e1-124">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="c70e1-125">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="c70e1-125">**studentEnrollment**</span></span> | [<span data-ttu-id="c70e1-126">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c70e1-126">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c70e1-127">学生登録のカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="c70e1-127">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="c70e1-128">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="c70e1-128">**teacherRoster**</span></span> | [<span data-ttu-id="c70e1-129">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c70e1-129">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="c70e1-130">教師名簿のカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="c70e1-130">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="c70e1-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c70e1-131">JSON representation</span></span>
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
