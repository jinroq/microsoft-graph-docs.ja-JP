---
title: educationExcelResource リソースの種類
description: 'EducationResource のサブクラス。 このリソースの種類は、Excel ドキュメントを表します。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ef85a92b2629e8a652ce59210018725d6afecb9a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972748"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="935e3-104">educationExcelResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="935e3-104">educationExcelResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="935e3-105">[EducationResource](educationresource.md)のサブクラス。</span><span class="sxs-lookup"><span data-stu-id="935e3-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="935e3-106">このリソースの種類は、Excel ドキュメントを表します。</span><span class="sxs-lookup"><span data-stu-id="935e3-106">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="935e3-107">**注:** Excel ファイルは、このリソースが属する assignment または送信オブジェクトに関連付けられたリソースフォルダーにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="935e3-107">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="935e3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="935e3-108">Properties</span></span>
| <span data-ttu-id="935e3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="935e3-109">Property</span></span>     | <span data-ttu-id="935e3-110">型</span><span class="sxs-lookup"><span data-stu-id="935e3-110">Type</span></span>   |<span data-ttu-id="935e3-111">説明</span><span class="sxs-lookup"><span data-stu-id="935e3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="935e3-112">fileUrl</span><span class="sxs-lookup"><span data-stu-id="935e3-112">fileUrl</span></span>|<span data-ttu-id="935e3-113">String</span><span class="sxs-lookup"><span data-stu-id="935e3-113">String</span></span>|<span data-ttu-id="935e3-114">Excel ファイルオブジェクトへのポインター。</span><span class="sxs-lookup"><span data-stu-id="935e3-114">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="935e3-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="935e3-115">JSON representation</span></span>

<span data-ttu-id="935e3-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="935e3-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationExcelResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
