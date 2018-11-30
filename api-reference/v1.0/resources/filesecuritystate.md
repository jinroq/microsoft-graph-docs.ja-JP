---
title: fileSecurityState リソースの種類
description: アラートに関連するファイル (プロセスではない) に関する情報が含まれています。
ms.openlocfilehash: d1358d7fe0d5565845201781e32b3da14a89f412
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023989"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="09c19-103">fileSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09c19-103">fileSecurityState resource type</span></span>

<span data-ttu-id="09c19-104">アラートに関連するファイル (プロセスではない) に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="09c19-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="09c19-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09c19-105">Properties</span></span>

| <span data-ttu-id="09c19-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09c19-106">Property</span></span>   | <span data-ttu-id="09c19-107">型</span><span class="sxs-lookup"><span data-stu-id="09c19-107">Type</span></span>|<span data-ttu-id="09c19-108">説明</span><span class="sxs-lookup"><span data-stu-id="09c19-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09c19-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="09c19-109">fileHash</span></span>|[<span data-ttu-id="09c19-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="09c19-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="09c19-111">複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。</span><span class="sxs-lookup"><span data-stu-id="09c19-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="09c19-112">名前</span><span class="sxs-lookup"><span data-stu-id="09c19-112">name</span></span>|<span data-ttu-id="09c19-113">String</span><span class="sxs-lookup"><span data-stu-id="09c19-113">String</span></span>|<span data-ttu-id="09c19-114">ファイルの名前 (パス) です。</span><span class="sxs-lookup"><span data-stu-id="09c19-114">File name (without path).</span></span>|
|<span data-ttu-id="09c19-115">path</span><span class="sxs-lookup"><span data-stu-id="09c19-115">path</span></span>|<span data-ttu-id="09c19-116">String</span><span class="sxs-lookup"><span data-stu-id="09c19-116">String</span></span>|<span data-ttu-id="09c19-117">ファイルとイメージ ファイルのファイルの完全パスです。</span><span class="sxs-lookup"><span data-stu-id="09c19-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="09c19-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="09c19-118">riskScore</span></span>|<span data-ttu-id="09c19-119">String</span><span class="sxs-lookup"><span data-stu-id="09c19-119">String</span></span>|<span data-ttu-id="09c19-120">プロバイダー生成された計算されるリスクの警告ファイルのスコアです。</span><span class="sxs-lookup"><span data-stu-id="09c19-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="09c19-121">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="09c19-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09c19-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09c19-122">JSON representation</span></span>

<span data-ttu-id="09c19-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="09c19-123">The following is a JSON representation of the resource.</span></span>

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