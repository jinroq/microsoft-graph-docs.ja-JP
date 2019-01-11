---
title: resultInfo リソースの種類
description: ResultInfo 型です。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: ca814fd5c44f0f811099faed53354d08ce8befdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855280"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="4fcb0-103">resultInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4fcb0-103">resultInfo resource type</span></span>

> <span data-ttu-id="4fcb0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4fcb0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4fcb0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fcb0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4fcb0-106">ResultInfo 型です。</span><span class="sxs-lookup"><span data-stu-id="4fcb0-106">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="4fcb0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fcb0-107">Properties</span></span>

| <span data-ttu-id="4fcb0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fcb0-108">Property</span></span> | <span data-ttu-id="4fcb0-109">種類</span><span class="sxs-lookup"><span data-stu-id="4fcb0-109">Type</span></span>   | <span data-ttu-id="4fcb0-110">説明</span><span class="sxs-lookup"><span data-stu-id="4fcb0-110">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="4fcb0-111">code</span><span class="sxs-lookup"><span data-stu-id="4fcb0-111">code</span></span>     | <span data-ttu-id="4fcb0-112">String</span><span class="sxs-lookup"><span data-stu-id="4fcb0-112">String</span></span> | <span data-ttu-id="4fcb0-113">結果コード。</span><span class="sxs-lookup"><span data-stu-id="4fcb0-113">The result code.</span></span>     |
| <span data-ttu-id="4fcb0-114">message</span><span class="sxs-lookup"><span data-stu-id="4fcb0-114">message</span></span>  | <span data-ttu-id="4fcb0-115">String</span><span class="sxs-lookup"><span data-stu-id="4fcb0-115">String</span></span> | <span data-ttu-id="4fcb0-116">メッセージ。</span><span class="sxs-lookup"><span data-stu-id="4fcb0-116">The message.</span></span>         |
| <span data-ttu-id="4fcb0-117">サブコード</span><span class="sxs-lookup"><span data-stu-id="4fcb0-117">subCode</span></span>  | <span data-ttu-id="4fcb0-118">String</span><span class="sxs-lookup"><span data-stu-id="4fcb0-118">String</span></span> | <span data-ttu-id="4fcb0-119">結果のサブ コードです。</span><span class="sxs-lookup"><span data-stu-id="4fcb0-119">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4fcb0-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4fcb0-120">JSON representation</span></span>

<span data-ttu-id="4fcb0-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4fcb0-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example-error-result"></a><span data-ttu-id="4fcb0-122">エラーの結果の例</span><span class="sxs-lookup"><span data-stu-id="4fcb0-122">Example Error result</span></span>

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

## <a name="example-generic-success-result"></a><span data-ttu-id="4fcb0-123">汎用的な成功の結果の例</span><span class="sxs-lookup"><span data-stu-id="4fcb0-123">Example Generic success result</span></span>

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

## <a name="example-record-success-result"></a><span data-ttu-id="4fcb0-124">レコードの成功の結果の例</span><span class="sxs-lookup"><span data-stu-id="4fcb0-124">Example Record Success result</span></span>

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
