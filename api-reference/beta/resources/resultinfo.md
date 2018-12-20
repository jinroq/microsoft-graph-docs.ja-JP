---
title: resultInfo リソースの種類
description: ResultInfo 型です。
author: VinodRavichandran
ms.openlocfilehash: db208ed214213ec906dac18b65140f010014fc6c
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380409"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="96d55-103">resultInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96d55-103">resultInfo resource type</span></span>

> <span data-ttu-id="96d55-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="96d55-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96d55-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96d55-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96d55-106">ResultInfo 型です。</span><span class="sxs-lookup"><span data-stu-id="96d55-106">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="96d55-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96d55-107">Properties</span></span>

| <span data-ttu-id="96d55-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96d55-108">Property</span></span> | <span data-ttu-id="96d55-109">型</span><span class="sxs-lookup"><span data-stu-id="96d55-109">Type</span></span>   | <span data-ttu-id="96d55-110">説明</span><span class="sxs-lookup"><span data-stu-id="96d55-110">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="96d55-111">code</span><span class="sxs-lookup"><span data-stu-id="96d55-111">code</span></span>     | <span data-ttu-id="96d55-112">String</span><span class="sxs-lookup"><span data-stu-id="96d55-112">String</span></span> | <span data-ttu-id="96d55-113">結果コード。</span><span class="sxs-lookup"><span data-stu-id="96d55-113">The result code.</span></span>     |
| <span data-ttu-id="96d55-114">message</span><span class="sxs-lookup"><span data-stu-id="96d55-114">message</span></span>  | <span data-ttu-id="96d55-115">String</span><span class="sxs-lookup"><span data-stu-id="96d55-115">String</span></span> | <span data-ttu-id="96d55-116">メッセージ。</span><span class="sxs-lookup"><span data-stu-id="96d55-116">The message.</span></span>         |
| <span data-ttu-id="96d55-117">サブコード</span><span class="sxs-lookup"><span data-stu-id="96d55-117">subCode</span></span>  | <span data-ttu-id="96d55-118">String</span><span class="sxs-lookup"><span data-stu-id="96d55-118">String</span></span> | <span data-ttu-id="96d55-119">結果のサブ コードです。</span><span class="sxs-lookup"><span data-stu-id="96d55-119">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="96d55-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96d55-120">JSON representation</span></span>

<span data-ttu-id="96d55-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96d55-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example-error-result"></a><span data-ttu-id="96d55-122">エラーの結果の例</span><span class="sxs-lookup"><span data-stu-id="96d55-122">Example Error result</span></span>

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

## <a name="example-generic-success-result"></a><span data-ttu-id="96d55-123">汎用的な成功の結果の例</span><span class="sxs-lookup"><span data-stu-id="96d55-123">Example Generic success result</span></span>

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

## <a name="example-record-success-result"></a><span data-ttu-id="96d55-124">レコードの成功の結果の例</span><span class="sxs-lookup"><span data-stu-id="96d55-124">Example Record Success result</span></span>

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
