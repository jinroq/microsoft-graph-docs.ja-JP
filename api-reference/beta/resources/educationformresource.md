---
title: educationFormResource リソースの種類
description: educationResource のサブクラス。 このリソースはフォームです。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3f2747d94c80732091db06294b26546afc567e03
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334266"
---
# <a name="educationformresource-resource-type"></a><span data-ttu-id="02d67-104">educationFormResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="02d67-104">educationFormResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02d67-105">[educationResource](educationresource.md)のサブクラス。</span><span class="sxs-lookup"><span data-stu-id="02d67-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="02d67-106">このリソースはフォームです。</span><span class="sxs-lookup"><span data-stu-id="02d67-106">This resource is a form.</span></span>


## <a name="properties"></a><span data-ttu-id="02d67-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02d67-107">Properties</span></span>
| <span data-ttu-id="02d67-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02d67-108">Property</span></span>     | <span data-ttu-id="02d67-109">型</span><span class="sxs-lookup"><span data-stu-id="02d67-109">Type</span></span>   |<span data-ttu-id="02d67-110">説明</span><span class="sxs-lookup"><span data-stu-id="02d67-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02d67-111">originalFormId</span><span class="sxs-lookup"><span data-stu-id="02d67-111">originalFormId</span></span>|<span data-ttu-id="02d67-112">String</span><span class="sxs-lookup"><span data-stu-id="02d67-112">String</span></span>|<span data-ttu-id="02d67-113">フォームの元の id。</span><span class="sxs-lookup"><span data-stu-id="02d67-113">Original id of the Form.</span></span>|
|<span data-ttu-id="02d67-114">formId</span><span class="sxs-lookup"><span data-stu-id="02d67-114">formId</span></span>|<span data-ttu-id="02d67-115">String</span><span class="sxs-lookup"><span data-stu-id="02d67-115">String</span></span>|<span data-ttu-id="02d67-116">フォームの Id。</span><span class="sxs-lookup"><span data-stu-id="02d67-116">Id of the Form.</span></span>|
|<span data-ttu-id="02d67-117">isgroupform</span><span class="sxs-lookup"><span data-stu-id="02d67-117">isGroupForm</span></span>|<span data-ttu-id="02d67-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="02d67-118">Boolean</span></span>|<span data-ttu-id="02d67-119">フォームがクラスグループに属しているかどうか。</span><span class="sxs-lookup"><span data-stu-id="02d67-119">Whether the Form belongs to a class group.</span></span>|
|<span data-ttu-id="02d67-120">viewurl</span><span class="sxs-lookup"><span data-stu-id="02d67-120">viewUrl</span></span>|<span data-ttu-id="02d67-121">String</span><span class="sxs-lookup"><span data-stu-id="02d67-121">String</span></span>|<span data-ttu-id="02d67-122">フォームの学生の URL。</span><span class="sxs-lookup"><span data-stu-id="02d67-122">Student URL for the Form.</span></span>|
|<span data-ttu-id="02d67-123">viewurl</span><span class="sxs-lookup"><span data-stu-id="02d67-123">viewUrl</span></span>|<span data-ttu-id="02d67-124">String</span><span class="sxs-lookup"><span data-stu-id="02d67-124">String</span></span>|<span data-ttu-id="02d67-125">フォームの学生の URL。</span><span class="sxs-lookup"><span data-stu-id="02d67-125">Student URL for the Form.</span></span>|
|<span data-ttu-id="02d67-126">editurl</span><span class="sxs-lookup"><span data-stu-id="02d67-126">editUrl</span></span>|<span data-ttu-id="02d67-127">String</span><span class="sxs-lookup"><span data-stu-id="02d67-127">String</span></span>|<span data-ttu-id="02d67-128">フォームの教師 URL。</span><span class="sxs-lookup"><span data-stu-id="02d67-128">Teacher URL for the Form.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02d67-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="02d67-129">JSON representation</span></span>

<span data-ttu-id="02d67-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="02d67-130">The following is a JSON representation of the resource.</span></span>

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
