---
title: fileSecurityState リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 485addfda2707c8848c44c839f9593378943f327
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526957"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="03a29-104">fileSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="03a29-104">fileSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03a29-105">アラートに関連するファイル (プロセスではない) に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="03a29-105">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="03a29-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03a29-106">Properties</span></span>

| <span data-ttu-id="03a29-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03a29-107">Property</span></span>   | <span data-ttu-id="03a29-108">型</span><span class="sxs-lookup"><span data-stu-id="03a29-108">Type</span></span>|<span data-ttu-id="03a29-109">説明</span><span class="sxs-lookup"><span data-stu-id="03a29-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03a29-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="03a29-110">fileHash</span></span>|[<span data-ttu-id="03a29-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="03a29-111">fileHash</span></span>](filehash.md)|<span data-ttu-id="03a29-112">複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。</span><span class="sxs-lookup"><span data-stu-id="03a29-112">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="03a29-113">name</span><span class="sxs-lookup"><span data-stu-id="03a29-113">name</span></span>|<span data-ttu-id="03a29-114">String</span><span class="sxs-lookup"><span data-stu-id="03a29-114">String</span></span>|<span data-ttu-id="03a29-115">ファイルの名前 (パス) です。</span><span class="sxs-lookup"><span data-stu-id="03a29-115">File name (without path).</span></span>|
|<span data-ttu-id="03a29-116">path</span><span class="sxs-lookup"><span data-stu-id="03a29-116">path</span></span>|<span data-ttu-id="03a29-117">String</span><span class="sxs-lookup"><span data-stu-id="03a29-117">String</span></span>|<span data-ttu-id="03a29-118">ファイルとイメージ ファイルのファイルの完全パスです。</span><span class="sxs-lookup"><span data-stu-id="03a29-118">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="03a29-119">riskScore</span><span class="sxs-lookup"><span data-stu-id="03a29-119">riskScore</span></span>|<span data-ttu-id="03a29-120">String</span><span class="sxs-lookup"><span data-stu-id="03a29-120">String</span></span>|<span data-ttu-id="03a29-121">プロバイダー生成された計算されるリスクの警告ファイルのスコアです。</span><span class="sxs-lookup"><span data-stu-id="03a29-121">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="03a29-122">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="03a29-122">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03a29-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03a29-123">JSON representation</span></span>

<span data-ttu-id="03a29-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="03a29-124">The following is a JSON representation of the resource.</span></span>

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
