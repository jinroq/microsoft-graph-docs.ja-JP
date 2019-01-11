---
title: fileSecurityState リソースの種類
description: アラートに関連するファイル (プロセスではない) に関する情報が含まれています。
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894097"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="21a5b-103">fileSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="21a5b-103">fileSecurityState resource type</span></span>

<span data-ttu-id="21a5b-104">アラートに関連するファイル (プロセスではない) に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="21a5b-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="21a5b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21a5b-105">Properties</span></span>

| <span data-ttu-id="21a5b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21a5b-106">Property</span></span>   | <span data-ttu-id="21a5b-107">種類</span><span class="sxs-lookup"><span data-stu-id="21a5b-107">Type</span></span>|<span data-ttu-id="21a5b-108">説明</span><span class="sxs-lookup"><span data-stu-id="21a5b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21a5b-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="21a5b-109">fileHash</span></span>|[<span data-ttu-id="21a5b-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="21a5b-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="21a5b-111">複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。</span><span class="sxs-lookup"><span data-stu-id="21a5b-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="21a5b-112">名前</span><span class="sxs-lookup"><span data-stu-id="21a5b-112">name</span></span>|<span data-ttu-id="21a5b-113">String</span><span class="sxs-lookup"><span data-stu-id="21a5b-113">String</span></span>|<span data-ttu-id="21a5b-114">ファイルの名前 (パス) です。</span><span class="sxs-lookup"><span data-stu-id="21a5b-114">File name (without path).</span></span>|
|<span data-ttu-id="21a5b-115">path</span><span class="sxs-lookup"><span data-stu-id="21a5b-115">path</span></span>|<span data-ttu-id="21a5b-116">String</span><span class="sxs-lookup"><span data-stu-id="21a5b-116">String</span></span>|<span data-ttu-id="21a5b-117">ファイルとイメージ ファイルのファイルの完全パスです。</span><span class="sxs-lookup"><span data-stu-id="21a5b-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="21a5b-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="21a5b-118">riskScore</span></span>|<span data-ttu-id="21a5b-119">String</span><span class="sxs-lookup"><span data-stu-id="21a5b-119">String</span></span>|<span data-ttu-id="21a5b-120">プロバイダー生成された計算されるリスクの警告ファイルのスコアです。</span><span class="sxs-lookup"><span data-stu-id="21a5b-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="21a5b-121">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="21a5b-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21a5b-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21a5b-122">JSON representation</span></span>

<span data-ttu-id="21a5b-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="21a5b-123">The following is a JSON representation of the resource.</span></span>

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
