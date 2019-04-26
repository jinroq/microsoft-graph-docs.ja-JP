---
title: fileSecurityState リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 8709df89c1a8b82f2381ab450fa235ba325a9f88
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333755"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="7c271-104">fileSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7c271-104">fileSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c271-105">通知に関連するファイル (プロセスではない) に関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="7c271-105">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="7c271-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c271-106">Properties</span></span>

| <span data-ttu-id="7c271-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c271-107">Property</span></span>   | <span data-ttu-id="7c271-108">型</span><span class="sxs-lookup"><span data-stu-id="7c271-108">Type</span></span>|<span data-ttu-id="7c271-109">説明</span><span class="sxs-lookup"><span data-stu-id="7c271-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c271-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="7c271-110">fileHash</span></span>|[<span data-ttu-id="7c271-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="7c271-111">fileHash</span></span>](filehash.md)|<span data-ttu-id="7c271-112">ファイルハッシュを含む複合型 (暗号化と場所に依存)。</span><span class="sxs-lookup"><span data-stu-id="7c271-112">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="7c271-113">name</span><span class="sxs-lookup"><span data-stu-id="7c271-113">name</span></span>|<span data-ttu-id="7c271-114">String</span><span class="sxs-lookup"><span data-stu-id="7c271-114">String</span></span>|<span data-ttu-id="7c271-115">ファイル名 (パスなし)。</span><span class="sxs-lookup"><span data-stu-id="7c271-115">File name (without path).</span></span>|
|<span data-ttu-id="7c271-116">path</span><span class="sxs-lookup"><span data-stu-id="7c271-116">path</span></span>|<span data-ttu-id="7c271-117">String</span><span class="sxs-lookup"><span data-stu-id="7c271-117">String</span></span>|<span data-ttu-id="7c271-118">ファイル/イメージファイルの完全なファイルパス。</span><span class="sxs-lookup"><span data-stu-id="7c271-118">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="7c271-119">riskScore</span><span class="sxs-lookup"><span data-stu-id="7c271-119">riskScore</span></span>|<span data-ttu-id="7c271-120">String</span><span class="sxs-lookup"><span data-stu-id="7c271-120">String</span></span>|<span data-ttu-id="7c271-121">通知ファイルのプロバイダーが生成/計算したリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="7c271-121">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="7c271-122">推奨値の範囲0-1。パーセンテージに相当します。</span><span class="sxs-lookup"><span data-stu-id="7c271-122">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c271-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7c271-123">JSON representation</span></span>

<span data-ttu-id="7c271-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c271-124">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
