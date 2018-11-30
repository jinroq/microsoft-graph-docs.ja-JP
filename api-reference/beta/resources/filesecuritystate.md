---
title: fileSecurityState リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: cbf535dd6b30387afbe361389fa6bcfca1fc68fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073671"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="b212c-104">fileSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b212c-104">fileSecurityState resource type</span></span>

 > <span data-ttu-id="b212c-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b212c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b212c-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b212c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b212c-107">アラートに関連するファイル (プロセスではない) に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b212c-107">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="b212c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b212c-108">Properties</span></span>

| <span data-ttu-id="b212c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b212c-109">Property</span></span>   | <span data-ttu-id="b212c-110">型</span><span class="sxs-lookup"><span data-stu-id="b212c-110">Type</span></span>|<span data-ttu-id="b212c-111">説明</span><span class="sxs-lookup"><span data-stu-id="b212c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b212c-112">fileHash</span><span class="sxs-lookup"><span data-stu-id="b212c-112">fileHash</span></span>|[<span data-ttu-id="b212c-113">fileHash</span><span class="sxs-lookup"><span data-stu-id="b212c-113">fileHash</span></span>](filehash.md)|<span data-ttu-id="b212c-114">複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b212c-114">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="b212c-115">名前</span><span class="sxs-lookup"><span data-stu-id="b212c-115">name</span></span>|<span data-ttu-id="b212c-116">String</span><span class="sxs-lookup"><span data-stu-id="b212c-116">String</span></span>|<span data-ttu-id="b212c-117">ファイルの名前 (パス) です。</span><span class="sxs-lookup"><span data-stu-id="b212c-117">File name (without path).</span></span>|
|<span data-ttu-id="b212c-118">path</span><span class="sxs-lookup"><span data-stu-id="b212c-118">path</span></span>|<span data-ttu-id="b212c-119">String</span><span class="sxs-lookup"><span data-stu-id="b212c-119">String</span></span>|<span data-ttu-id="b212c-120">ファイルとイメージ ファイルのファイルの完全パスです。</span><span class="sxs-lookup"><span data-stu-id="b212c-120">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="b212c-121">riskScore</span><span class="sxs-lookup"><span data-stu-id="b212c-121">riskScore</span></span>|<span data-ttu-id="b212c-122">String</span><span class="sxs-lookup"><span data-stu-id="b212c-122">String</span></span>|<span data-ttu-id="b212c-123">プロバイダー生成された計算されるリスクの警告ファイルのスコアです。</span><span class="sxs-lookup"><span data-stu-id="b212c-123">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="b212c-124">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="b212c-124">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b212c-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b212c-125">JSON representation</span></span>

<span data-ttu-id="b212c-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b212c-126">The following is a JSON representation of the resource.</span></span>

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