---
title: fileSecurityState リソースの種類
description: 通知に関連するファイル (プロセスではない) に関する情報が含まれます。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6e6f30625412022006d88179e3192b1463c797c0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032495"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="a579c-103">fileSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a579c-103">fileSecurityState resource type</span></span>

<span data-ttu-id="a579c-104">通知に関連するファイル (プロセスではない) に関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a579c-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="a579c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a579c-105">Properties</span></span>

| <span data-ttu-id="a579c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a579c-106">Property</span></span>   | <span data-ttu-id="a579c-107">型</span><span class="sxs-lookup"><span data-stu-id="a579c-107">Type</span></span>|<span data-ttu-id="a579c-108">説明</span><span class="sxs-lookup"><span data-stu-id="a579c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a579c-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="a579c-109">fileHash</span></span>|[<span data-ttu-id="a579c-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="a579c-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="a579c-111">ファイルハッシュを含む複合型 (暗号化と場所に依存)。</span><span class="sxs-lookup"><span data-stu-id="a579c-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="a579c-112">name</span><span class="sxs-lookup"><span data-stu-id="a579c-112">name</span></span>|<span data-ttu-id="a579c-113">String</span><span class="sxs-lookup"><span data-stu-id="a579c-113">String</span></span>|<span data-ttu-id="a579c-114">ファイル名 (パスなし)。</span><span class="sxs-lookup"><span data-stu-id="a579c-114">File name (without path).</span></span>|
|<span data-ttu-id="a579c-115">path</span><span class="sxs-lookup"><span data-stu-id="a579c-115">path</span></span>|<span data-ttu-id="a579c-116">String</span><span class="sxs-lookup"><span data-stu-id="a579c-116">String</span></span>|<span data-ttu-id="a579c-117">ファイル/イメージファイルの完全なファイルパス。</span><span class="sxs-lookup"><span data-stu-id="a579c-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="a579c-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="a579c-118">riskScore</span></span>|<span data-ttu-id="a579c-119">String</span><span class="sxs-lookup"><span data-stu-id="a579c-119">String</span></span>|<span data-ttu-id="a579c-120">通知ファイルのプロバイダーが生成/計算したリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="a579c-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="a579c-121">推奨値の範囲0-1。パーセンテージに相当します。</span><span class="sxs-lookup"><span data-stu-id="a579c-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a579c-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a579c-122">JSON representation</span></span>

<span data-ttu-id="a579c-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a579c-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
