---
title: resultinfo リソースの種類
description: resultinfo 型。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 0c924798715448e87c30cf2b65cc923c6ddc20bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562994"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="2dfd7-103">resultinfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2dfd7-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dfd7-104">resultinfo 型。</span><span class="sxs-lookup"><span data-stu-id="2dfd7-104">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="2dfd7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2dfd7-105">Properties</span></span>

| <span data-ttu-id="2dfd7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2dfd7-106">Property</span></span> | <span data-ttu-id="2dfd7-107">型</span><span class="sxs-lookup"><span data-stu-id="2dfd7-107">Type</span></span>   | <span data-ttu-id="2dfd7-108">説明</span><span class="sxs-lookup"><span data-stu-id="2dfd7-108">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="2dfd7-109">code</span><span class="sxs-lookup"><span data-stu-id="2dfd7-109">code</span></span>     | <span data-ttu-id="2dfd7-110">String</span><span class="sxs-lookup"><span data-stu-id="2dfd7-110">String</span></span> | <span data-ttu-id="2dfd7-111">結果コード。</span><span class="sxs-lookup"><span data-stu-id="2dfd7-111">The result code.</span></span>     |
| <span data-ttu-id="2dfd7-112">message</span><span class="sxs-lookup"><span data-stu-id="2dfd7-112">message</span></span>  | <span data-ttu-id="2dfd7-113">String</span><span class="sxs-lookup"><span data-stu-id="2dfd7-113">String</span></span> | <span data-ttu-id="2dfd7-114">メッセージ。</span><span class="sxs-lookup"><span data-stu-id="2dfd7-114">The message.</span></span>         |
| <span data-ttu-id="2dfd7-115">subCode</span><span class="sxs-lookup"><span data-stu-id="2dfd7-115">subCode</span></span>  | <span data-ttu-id="2dfd7-116">String</span><span class="sxs-lookup"><span data-stu-id="2dfd7-116">String</span></span> | <span data-ttu-id="2dfd7-117">結果サブコード。</span><span class="sxs-lookup"><span data-stu-id="2dfd7-117">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2dfd7-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2dfd7-118">JSON representation</span></span>

<span data-ttu-id="2dfd7-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2dfd7-119">The following is a JSON representation of the resource.</span></span>

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

## <a name="example-error-result"></a><span data-ttu-id="2dfd7-120">エラー結果の例</span><span class="sxs-lookup"><span data-stu-id="2dfd7-120">Example Error result</span></span>

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

## <a name="example-generic-success-result"></a><span data-ttu-id="2dfd7-121">一般的な成功結果の例</span><span class="sxs-lookup"><span data-stu-id="2dfd7-121">Example Generic success result</span></span>

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

## <a name="example-record-success-result"></a><span data-ttu-id="2dfd7-122">レコード成功の例</span><span class="sxs-lookup"><span data-stu-id="2dfd7-122">Example Record Success result</span></span>

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
  "suppressions": []
}
-->
