---
title: educationFormResource リソースの種類
description: EducationResource のサブクラス。 このリソースはフォームです。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d2e10ea6db0236b7deff3581c2e1b4f97c589045
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972720"
---
# <a name="educationformresource-resource-type"></a><span data-ttu-id="1e23f-104">educationFormResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1e23f-104">educationFormResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e23f-105">[EducationResource](educationresource.md)のサブクラス。</span><span class="sxs-lookup"><span data-stu-id="1e23f-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="1e23f-106">このリソースはフォームです。</span><span class="sxs-lookup"><span data-stu-id="1e23f-106">This resource is a form.</span></span>


## <a name="properties"></a><span data-ttu-id="1e23f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e23f-107">Properties</span></span>
| <span data-ttu-id="1e23f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e23f-108">Property</span></span>     | <span data-ttu-id="1e23f-109">型</span><span class="sxs-lookup"><span data-stu-id="1e23f-109">Type</span></span>   |<span data-ttu-id="1e23f-110">説明</span><span class="sxs-lookup"><span data-stu-id="1e23f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e23f-111">originalFormId</span><span class="sxs-lookup"><span data-stu-id="1e23f-111">originalFormId</span></span>|<span data-ttu-id="1e23f-112">String</span><span class="sxs-lookup"><span data-stu-id="1e23f-112">String</span></span>|<span data-ttu-id="1e23f-113">フォームの元の id。</span><span class="sxs-lookup"><span data-stu-id="1e23f-113">Original id of the Form.</span></span>|
|<span data-ttu-id="1e23f-114">formId</span><span class="sxs-lookup"><span data-stu-id="1e23f-114">formId</span></span>|<span data-ttu-id="1e23f-115">String</span><span class="sxs-lookup"><span data-stu-id="1e23f-115">String</span></span>|<span data-ttu-id="1e23f-116">フォームの Id。</span><span class="sxs-lookup"><span data-stu-id="1e23f-116">Id of the Form.</span></span>|
|<span data-ttu-id="1e23f-117">isGroupForm</span><span class="sxs-lookup"><span data-stu-id="1e23f-117">isGroupForm</span></span>|<span data-ttu-id="1e23f-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e23f-118">Boolean</span></span>|<span data-ttu-id="1e23f-119">フォームがクラスグループに属しているかどうか。</span><span class="sxs-lookup"><span data-stu-id="1e23f-119">Whether the Form belongs to a class group.</span></span>|
|<span data-ttu-id="1e23f-120">viewUrl</span><span class="sxs-lookup"><span data-stu-id="1e23f-120">viewUrl</span></span>|<span data-ttu-id="1e23f-121">String</span><span class="sxs-lookup"><span data-stu-id="1e23f-121">String</span></span>|<span data-ttu-id="1e23f-122">フォームの学生の URL。</span><span class="sxs-lookup"><span data-stu-id="1e23f-122">Student URL for the Form.</span></span>|
|<span data-ttu-id="1e23f-123">viewUrl</span><span class="sxs-lookup"><span data-stu-id="1e23f-123">viewUrl</span></span>|<span data-ttu-id="1e23f-124">String</span><span class="sxs-lookup"><span data-stu-id="1e23f-124">String</span></span>|<span data-ttu-id="1e23f-125">フォームの学生の URL。</span><span class="sxs-lookup"><span data-stu-id="1e23f-125">Student URL for the Form.</span></span>|
|<span data-ttu-id="1e23f-126">editUrl</span><span class="sxs-lookup"><span data-stu-id="1e23f-126">editUrl</span></span>|<span data-ttu-id="1e23f-127">String</span><span class="sxs-lookup"><span data-stu-id="1e23f-127">String</span></span>|<span data-ttu-id="1e23f-128">フォームの教師 URL。</span><span class="sxs-lookup"><span data-stu-id="1e23f-128">Teacher URL for the Form.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e23f-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e23f-129">JSON representation</span></span>

<span data-ttu-id="1e23f-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e23f-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFormResource"
}-->

```json
{
  "originalFormId": "String",
  "formId": "String",
  "isGroupForm": "Boolean",
  "viewUrl": "String",
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
  "suppressions": []
}
-->
