---
title: educationExcelResource リソースの種類
description: 'EducationResource のサブクラスです。 この種類のリソースでは、Excel ドキュメントを表します。  '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 7f772f7911667c76e64c31a856f3a9f8b6f3e6ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858101"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="aa4ab-104">educationExcelResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aa4ab-104">educationExcelResource resource type</span></span>

> <span data-ttu-id="aa4ab-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aa4ab-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa4ab-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa4ab-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa4ab-107">[EducationResource](educationresource.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="aa4ab-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="aa4ab-108">この種類のリソースでは、Excel ドキュメントを表します。</span><span class="sxs-lookup"><span data-stu-id="aa4ab-108">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="aa4ab-109">**注:** Excel ファイルは、このリソースが所属する割り当てまたは提出書類のオブジェクトに関連付けられているリソースのフォルダーにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="aa4ab-109">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="aa4ab-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa4ab-110">Properties</span></span>
| <span data-ttu-id="aa4ab-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa4ab-111">Property</span></span>     | <span data-ttu-id="aa4ab-112">種類</span><span class="sxs-lookup"><span data-stu-id="aa4ab-112">Type</span></span>   |<span data-ttu-id="aa4ab-113">説明</span><span class="sxs-lookup"><span data-stu-id="aa4ab-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa4ab-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="aa4ab-114">fileUrl</span></span>|<span data-ttu-id="aa4ab-115">String</span><span class="sxs-lookup"><span data-stu-id="aa4ab-115">String</span></span>|<span data-ttu-id="aa4ab-116">Excel ファイルのオブジェクトへのポインター。</span><span class="sxs-lookup"><span data-stu-id="aa4ab-116">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa4ab-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa4ab-117">JSON representation</span></span>

<span data-ttu-id="aa4ab-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aa4ab-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
