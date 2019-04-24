---
title: fileSecurityState リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 485addfda2707c8848c44c839f9593378943f327
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506409"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="77238-104">fileSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="77238-104">fileSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77238-105">通知に関連するファイル (プロセスではない) に関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="77238-105">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="77238-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77238-106">Properties</span></span>

| <span data-ttu-id="77238-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77238-107">Property</span></span>   | <span data-ttu-id="77238-108">型</span><span class="sxs-lookup"><span data-stu-id="77238-108">Type</span></span>|<span data-ttu-id="77238-109">説明</span><span class="sxs-lookup"><span data-stu-id="77238-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77238-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="77238-110">fileHash</span></span>|[<span data-ttu-id="77238-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="77238-111">fileHash</span></span>](filehash.md)|<span data-ttu-id="77238-112">ファイルハッシュを含む複合型 (暗号化と場所に依存)。</span><span class="sxs-lookup"><span data-stu-id="77238-112">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="77238-113">name</span><span class="sxs-lookup"><span data-stu-id="77238-113">name</span></span>|<span data-ttu-id="77238-114">String</span><span class="sxs-lookup"><span data-stu-id="77238-114">String</span></span>|<span data-ttu-id="77238-115">ファイル名 (パスなし)。</span><span class="sxs-lookup"><span data-stu-id="77238-115">File name (without path).</span></span>|
|<span data-ttu-id="77238-116">path</span><span class="sxs-lookup"><span data-stu-id="77238-116">path</span></span>|<span data-ttu-id="77238-117">String</span><span class="sxs-lookup"><span data-stu-id="77238-117">String</span></span>|<span data-ttu-id="77238-118">ファイル/イメージファイルの完全なファイルパス。</span><span class="sxs-lookup"><span data-stu-id="77238-118">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="77238-119">riskScore</span><span class="sxs-lookup"><span data-stu-id="77238-119">riskScore</span></span>|<span data-ttu-id="77238-120">String</span><span class="sxs-lookup"><span data-stu-id="77238-120">String</span></span>|<span data-ttu-id="77238-121">通知ファイルのプロバイダーが生成/計算したリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="77238-121">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="77238-122">推奨値の範囲0-1。パーセンテージに相当します。</span><span class="sxs-lookup"><span data-stu-id="77238-122">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77238-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="77238-123">JSON representation</span></span>

<span data-ttu-id="77238-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="77238-124">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/filesecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
