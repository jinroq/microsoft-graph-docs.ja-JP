---
title: educationFormResource リソースの種類
description: educationResource のサブクラス。 このリソースはフォームです。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5e0b03eeea8c0e9d22a9f7279c821f6d90211470
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2019
ms.locfileid: "30801023"
---
# <a name="educationformresource-resource-type"></a><span data-ttu-id="5edda-104">educationFormResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5edda-104">educationFormResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5edda-105">[educationResource](educationresource.md)のサブクラス。</span><span class="sxs-lookup"><span data-stu-id="5edda-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="5edda-106">このリソースはフォームです。</span><span class="sxs-lookup"><span data-stu-id="5edda-106">This resource is a form.</span></span>


## <a name="properties"></a><span data-ttu-id="5edda-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5edda-107">Properties</span></span>
| <span data-ttu-id="5edda-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5edda-108">Property</span></span>     | <span data-ttu-id="5edda-109">型</span><span class="sxs-lookup"><span data-stu-id="5edda-109">Type</span></span>   |<span data-ttu-id="5edda-110">説明</span><span class="sxs-lookup"><span data-stu-id="5edda-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5edda-111">originalFormId</span><span class="sxs-lookup"><span data-stu-id="5edda-111">originalFormId</span></span>|<span data-ttu-id="5edda-112">String</span><span class="sxs-lookup"><span data-stu-id="5edda-112">String</span></span>|<span data-ttu-id="5edda-113">フォームの元の id。</span><span class="sxs-lookup"><span data-stu-id="5edda-113">Original id of the Form.</span></span>|
|<span data-ttu-id="5edda-114">formId</span><span class="sxs-lookup"><span data-stu-id="5edda-114">formId</span></span>|<span data-ttu-id="5edda-115">String</span><span class="sxs-lookup"><span data-stu-id="5edda-115">String</span></span>|<span data-ttu-id="5edda-116">フォームの Id。</span><span class="sxs-lookup"><span data-stu-id="5edda-116">Id of the Form.</span></span>|
|<span data-ttu-id="5edda-117">isgroupform</span><span class="sxs-lookup"><span data-stu-id="5edda-117">isGroupForm</span></span>|<span data-ttu-id="5edda-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="5edda-118">Boolean</span></span>|<span data-ttu-id="5edda-119">フォームがクラスグループに属しているかどうか。</span><span class="sxs-lookup"><span data-stu-id="5edda-119">Whether the Form belongs to a class group.</span></span>|
|<span data-ttu-id="5edda-120">viewurl</span><span class="sxs-lookup"><span data-stu-id="5edda-120">viewUrl</span></span>|<span data-ttu-id="5edda-121">String</span><span class="sxs-lookup"><span data-stu-id="5edda-121">String</span></span>|<span data-ttu-id="5edda-122">フォームの学生の URL。</span><span class="sxs-lookup"><span data-stu-id="5edda-122">Student URL for the Form.</span></span>|
|<span data-ttu-id="5edda-123">viewurl</span><span class="sxs-lookup"><span data-stu-id="5edda-123">viewUrl</span></span>|<span data-ttu-id="5edda-124">String</span><span class="sxs-lookup"><span data-stu-id="5edda-124">String</span></span>|<span data-ttu-id="5edda-125">フォームの学生の URL。</span><span class="sxs-lookup"><span data-stu-id="5edda-125">Student URL for the Form.</span></span>|
|<span data-ttu-id="5edda-126">editurl</span><span class="sxs-lookup"><span data-stu-id="5edda-126">editUrl</span></span>|<span data-ttu-id="5edda-127">String</span><span class="sxs-lookup"><span data-stu-id="5edda-127">String</span></span>|<span data-ttu-id="5edda-128">フォームの教師 URL。</span><span class="sxs-lookup"><span data-stu-id="5edda-128">Teacher URL for the Form.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5edda-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5edda-129">JSON representation</span></span>

<span data-ttu-id="5edda-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5edda-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFormResource"
}-->

```json
{
  "originalFormId": "String"
  "formId": "String"
  "isGroupForm": "Boolean"
  "viewUrl": "String"
  "editUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFormResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationformresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
