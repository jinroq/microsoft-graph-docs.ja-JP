---
title: resultInfo リソースの種類
description: ResultInfo 型です。
ms.openlocfilehash: 93dc08407608a87cbc1cfa027f5c8f20483834e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068565"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="aa68b-103">resultInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aa68b-103">resultInfo resource type</span></span>

> <span data-ttu-id="aa68b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aa68b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa68b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa68b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa68b-106">ResultInfo 型です。</span><span class="sxs-lookup"><span data-stu-id="aa68b-106">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="aa68b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa68b-107">Properties</span></span>

| <span data-ttu-id="aa68b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa68b-108">Property</span></span> | <span data-ttu-id="aa68b-109">型</span><span class="sxs-lookup"><span data-stu-id="aa68b-109">Type</span></span>   | <span data-ttu-id="aa68b-110">説明</span><span class="sxs-lookup"><span data-stu-id="aa68b-110">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="aa68b-111">code</span><span class="sxs-lookup"><span data-stu-id="aa68b-111">code</span></span>     | <span data-ttu-id="aa68b-112">String</span><span class="sxs-lookup"><span data-stu-id="aa68b-112">String</span></span> | <span data-ttu-id="aa68b-113">結果コード。</span><span class="sxs-lookup"><span data-stu-id="aa68b-113">The result code.</span></span>     |
| <span data-ttu-id="aa68b-114">message</span><span class="sxs-lookup"><span data-stu-id="aa68b-114">message</span></span>  | <span data-ttu-id="aa68b-115">String</span><span class="sxs-lookup"><span data-stu-id="aa68b-115">String</span></span> | <span data-ttu-id="aa68b-116">メッセージ。</span><span class="sxs-lookup"><span data-stu-id="aa68b-116">The message.</span></span>         |
| <span data-ttu-id="aa68b-117">サブコード</span><span class="sxs-lookup"><span data-stu-id="aa68b-117">subCode</span></span>  | <span data-ttu-id="aa68b-118">String</span><span class="sxs-lookup"><span data-stu-id="aa68b-118">String</span></span> | <span data-ttu-id="aa68b-119">結果のサブ コードです。</span><span class="sxs-lookup"><span data-stu-id="aa68b-119">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aa68b-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa68b-120">JSON representation</span></span>

<span data-ttu-id="aa68b-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aa68b-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example-error-result"></a><span data-ttu-id="aa68b-122">エラーの結果の例</span><span class="sxs-lookup"><span data-stu-id="aa68b-122">Example Error result</span></span>

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

## <a name="example-generic-success-result"></a><span data-ttu-id="aa68b-123">汎用的な成功の結果の例</span><span class="sxs-lookup"><span data-stu-id="aa68b-123">Example Generic success result</span></span>

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

## <a name="example-record-success-result"></a><span data-ttu-id="aa68b-124">レコードの成功の結果の例</span><span class="sxs-lookup"><span data-stu-id="aa68b-124">Example Record Success result</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
