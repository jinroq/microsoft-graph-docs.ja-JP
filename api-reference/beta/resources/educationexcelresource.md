---
title: educationExcelResource リソースの種類
description: 'EducationResource のサブクラスです。 この種類のリソースでは、Excel ドキュメントを表します。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 14d7823f166ca12d202a6561bc9fe7b158ab7476
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522421"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="9dbc7-104">educationExcelResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9dbc7-104">educationExcelResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dbc7-105">[EducationResource](educationresource.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="9dbc7-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="9dbc7-106">この種類のリソースでは、Excel ドキュメントを表します。</span><span class="sxs-lookup"><span data-stu-id="9dbc7-106">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="9dbc7-107">**注:** Excel ファイルは、このリソースが所属する割り当てまたは提出書類のオブジェクトに関連付けられているリソースのフォルダーにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9dbc7-107">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="9dbc7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9dbc7-108">Properties</span></span>
| <span data-ttu-id="9dbc7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9dbc7-109">Property</span></span>     | <span data-ttu-id="9dbc7-110">型</span><span class="sxs-lookup"><span data-stu-id="9dbc7-110">Type</span></span>   |<span data-ttu-id="9dbc7-111">説明</span><span class="sxs-lookup"><span data-stu-id="9dbc7-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9dbc7-112">FileURL</span><span class="sxs-lookup"><span data-stu-id="9dbc7-112">fileUrl</span></span>|<span data-ttu-id="9dbc7-113">String</span><span class="sxs-lookup"><span data-stu-id="9dbc7-113">String</span></span>|<span data-ttu-id="9dbc7-114">Excel ファイルのオブジェクトへのポインター。</span><span class="sxs-lookup"><span data-stu-id="9dbc7-114">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9dbc7-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9dbc7-115">JSON representation</span></span>

<span data-ttu-id="9dbc7-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9dbc7-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationexcelresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
