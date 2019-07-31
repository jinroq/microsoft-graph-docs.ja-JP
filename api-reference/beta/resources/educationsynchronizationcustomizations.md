---
title: educationSynchronizationCustomizations リソースの種類
description: 同期するエンティティのリストと、そのカスタマイズがあればそれを含みます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d31be9bd808f411c1e208ab953784fdefd65fdda
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972440"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="95604-103">educationSynchronizationCustomizations リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95604-103">educationSynchronizationCustomizations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95604-104">同期するエンティティのリストと、その[カスタマイズ](educationsynchronizationcustomization.md)があればそれを含みます。</span><span class="sxs-lookup"><span data-stu-id="95604-104">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="95604-105">**注:** 同期するプロパティのカスタマイズは、 **studentEnrollment**エンティティおよび**teacherRoster**エンティティには適用されません。</span><span class="sxs-lookup"><span data-stu-id="95604-105">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="95604-106">このリソースは、次のデータプロバイダーのメンバーです。</span><span class="sxs-lookup"><span data-stu-id="95604-106">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="95604-107">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="95604-107">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="95604-108">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="95604-108">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="95604-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95604-109">Properties</span></span>

| <span data-ttu-id="95604-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95604-110">Property</span></span> | <span data-ttu-id="95604-111">型</span><span class="sxs-lookup"><span data-stu-id="95604-111">Type</span></span> | <span data-ttu-id="95604-112">説明</span><span class="sxs-lookup"><span data-stu-id="95604-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="95604-113">**筆記**</span><span class="sxs-lookup"><span data-stu-id="95604-113">**school**</span></span> | [<span data-ttu-id="95604-114">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="95604-114">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="95604-115">学校エンティティのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="95604-115">Customization for a school entity.</span></span>        |
| <span data-ttu-id="95604-116">**セクション**</span><span class="sxs-lookup"><span data-stu-id="95604-116">**section**</span></span> | [<span data-ttu-id="95604-117">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="95604-117">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="95604-118">セクションエンティティのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="95604-118">Customization for a section entity.</span></span>         |
| <span data-ttu-id="95604-119">**学生**</span><span class="sxs-lookup"><span data-stu-id="95604-119">**student**</span></span> | [<span data-ttu-id="95604-120">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="95604-120">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="95604-121">学生エンティティのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="95604-121">Customization for a student entity.</span></span>         |
| <span data-ttu-id="95604-122">**teacher**</span><span class="sxs-lookup"><span data-stu-id="95604-122">**teacher**</span></span> | [<span data-ttu-id="95604-123">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="95604-123">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="95604-124">教師エンティティのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="95604-124">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="95604-125">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="95604-125">**studentEnrollment**</span></span> | [<span data-ttu-id="95604-126">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="95604-126">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="95604-127">学生登録のカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="95604-127">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="95604-128">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="95604-128">**teacherRoster**</span></span> | [<span data-ttu-id="95604-129">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="95604-129">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="95604-130">教師名簿のカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="95604-130">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="95604-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95604-131">JSON representation</span></span>
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
