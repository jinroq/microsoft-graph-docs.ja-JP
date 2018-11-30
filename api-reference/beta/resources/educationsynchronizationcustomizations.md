---
title: educationSynchronizationCustomizations リソースの種類
description: 存在する場合は、同期と、カスタマイズするエンティティの一覧に含まれています。
ms.openlocfilehash: d694c5ea1136d38e11ff3f1aca0ad0fde34b9d02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070741"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="00613-103">educationSynchronizationCustomizations リソースの種類</span><span class="sxs-lookup"><span data-stu-id="00613-103">educationSynchronizationCustomizations resource type</span></span>

> <span data-ttu-id="00613-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="00613-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00613-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00613-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00613-106">存在する場合は、同期を[カスタマイズ](educationsynchronizationcustomization.md)して、エンティティの一覧に含まれています。</span><span class="sxs-lookup"><span data-stu-id="00613-106">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="00613-107">**注:** 同期プロパティのカスタマイズは、 **studentEnrollment**と**teacherRoster**のエンティティには適用されません。</span><span class="sxs-lookup"><span data-stu-id="00613-107">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="00613-108">このリソースは、次のデータ プロバイダーのメンバーです。</span><span class="sxs-lookup"><span data-stu-id="00613-108">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="00613-109">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="00613-109">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="00613-110">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="00613-110">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="00613-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00613-111">Properties</span></span>

| <span data-ttu-id="00613-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00613-112">Property</span></span> | <span data-ttu-id="00613-113">型</span><span class="sxs-lookup"><span data-stu-id="00613-113">Type</span></span> | <span data-ttu-id="00613-114">説明</span><span class="sxs-lookup"><span data-stu-id="00613-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="00613-115">**学校**</span><span class="sxs-lookup"><span data-stu-id="00613-115">**school**</span></span> | [<span data-ttu-id="00613-116">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="00613-116">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="00613-117">学校のエンティティのカスタマイズです。</span><span class="sxs-lookup"><span data-stu-id="00613-117">Customization for a school entity.</span></span>        |
| <span data-ttu-id="00613-118">**section**</span><span class="sxs-lookup"><span data-stu-id="00613-118">**section**</span></span> | [<span data-ttu-id="00613-119">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="00613-119">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="00613-120">セクション エンティティをカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="00613-120">Customization for a section entity.</span></span>         |
| <span data-ttu-id="00613-121">**受講者用**</span><span class="sxs-lookup"><span data-stu-id="00613-121">**student**</span></span> | [<span data-ttu-id="00613-122">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="00613-122">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="00613-123">受講者用のエンティティのカスタマイズです。</span><span class="sxs-lookup"><span data-stu-id="00613-123">Customization for a student entity.</span></span>         |
| <span data-ttu-id="00613-124">**teacher**</span><span class="sxs-lookup"><span data-stu-id="00613-124">**teacher**</span></span> | [<span data-ttu-id="00613-125">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="00613-125">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="00613-126">先生のエンティティのカスタマイズです。</span><span class="sxs-lookup"><span data-stu-id="00613-126">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="00613-127">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="00613-127">**studentEnrollment**</span></span> | [<span data-ttu-id="00613-128">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="00613-128">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="00613-129">受講者の登録用にカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="00613-129">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="00613-130">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="00613-130">**teacherRoster**</span></span> | [<span data-ttu-id="00613-131">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="00613-131">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="00613-132">教師名簿をカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="00613-132">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="00613-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="00613-133">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomizations"
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
