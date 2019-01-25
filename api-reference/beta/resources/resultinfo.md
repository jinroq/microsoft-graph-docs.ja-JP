---
title: resultInfo リソースの種類
description: ResultInfo 型です。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 0c924798715448e87c30cf2b65cc923c6ddc20bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521083"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="ebf27-103">resultInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ebf27-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebf27-104">ResultInfo 型です。</span><span class="sxs-lookup"><span data-stu-id="ebf27-104">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="ebf27-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebf27-105">Properties</span></span>

| <span data-ttu-id="ebf27-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebf27-106">Property</span></span> | <span data-ttu-id="ebf27-107">型</span><span class="sxs-lookup"><span data-stu-id="ebf27-107">Type</span></span>   | <span data-ttu-id="ebf27-108">説明</span><span class="sxs-lookup"><span data-stu-id="ebf27-108">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="ebf27-109">code</span><span class="sxs-lookup"><span data-stu-id="ebf27-109">code</span></span>     | <span data-ttu-id="ebf27-110">String</span><span class="sxs-lookup"><span data-stu-id="ebf27-110">String</span></span> | <span data-ttu-id="ebf27-111">結果コード。</span><span class="sxs-lookup"><span data-stu-id="ebf27-111">The result code.</span></span>     |
| <span data-ttu-id="ebf27-112">message</span><span class="sxs-lookup"><span data-stu-id="ebf27-112">message</span></span>  | <span data-ttu-id="ebf27-113">String</span><span class="sxs-lookup"><span data-stu-id="ebf27-113">String</span></span> | <span data-ttu-id="ebf27-114">メッセージ。</span><span class="sxs-lookup"><span data-stu-id="ebf27-114">The message.</span></span>         |
| <span data-ttu-id="ebf27-115">サブコード</span><span class="sxs-lookup"><span data-stu-id="ebf27-115">subCode</span></span>  | <span data-ttu-id="ebf27-116">String</span><span class="sxs-lookup"><span data-stu-id="ebf27-116">String</span></span> | <span data-ttu-id="ebf27-117">結果のサブ コードです。</span><span class="sxs-lookup"><span data-stu-id="ebf27-117">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ebf27-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ebf27-118">JSON representation</span></span>

<span data-ttu-id="ebf27-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ebf27-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "String",
  "message": "String",
  "subCode": "String"
}
```

## <a name="example-error-result"></a><span data-ttu-id="ebf27-120">エラーの結果の例</span><span class="sxs-lookup"><span data-stu-id="ebf27-120">Example Error result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "100",
  "message": "Internal Server Error.",
  "subCode": "20"
}
```

## <a name="example-generic-success-result"></a><span data-ttu-id="ebf27-121">汎用的な成功の結果の例</span><span class="sxs-lookup"><span data-stu-id="ebf27-121">Example Generic success result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "0"
}
```

## <a name="example-record-success-result"></a><span data-ttu-id="ebf27-122">レコードの成功の結果の例</span><span class="sxs-lookup"><span data-stu-id="ebf27-122">Example Record Success result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "completedSilenceDetected"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resultinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
