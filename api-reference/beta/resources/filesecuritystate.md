---
title: fileSecurityState リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 9d18021591b24d26577e41897111b90310746d18
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869504"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="17949-104">fileSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="17949-104">fileSecurityState resource type</span></span>

 > <span data-ttu-id="17949-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="17949-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17949-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17949-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17949-107">アラートに関連するファイル (プロセスではない) に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="17949-107">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="17949-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17949-108">Properties</span></span>

| <span data-ttu-id="17949-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17949-109">Property</span></span>   | <span data-ttu-id="17949-110">種類</span><span class="sxs-lookup"><span data-stu-id="17949-110">Type</span></span>|<span data-ttu-id="17949-111">説明</span><span class="sxs-lookup"><span data-stu-id="17949-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17949-112">fileHash</span><span class="sxs-lookup"><span data-stu-id="17949-112">fileHash</span></span>|[<span data-ttu-id="17949-113">fileHash</span><span class="sxs-lookup"><span data-stu-id="17949-113">fileHash</span></span>](filehash.md)|<span data-ttu-id="17949-114">複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。</span><span class="sxs-lookup"><span data-stu-id="17949-114">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="17949-115">名前</span><span class="sxs-lookup"><span data-stu-id="17949-115">name</span></span>|<span data-ttu-id="17949-116">String</span><span class="sxs-lookup"><span data-stu-id="17949-116">String</span></span>|<span data-ttu-id="17949-117">ファイルの名前 (パス) です。</span><span class="sxs-lookup"><span data-stu-id="17949-117">File name (without path).</span></span>|
|<span data-ttu-id="17949-118">path</span><span class="sxs-lookup"><span data-stu-id="17949-118">path</span></span>|<span data-ttu-id="17949-119">String</span><span class="sxs-lookup"><span data-stu-id="17949-119">String</span></span>|<span data-ttu-id="17949-120">ファイルとイメージ ファイルのファイルの完全パスです。</span><span class="sxs-lookup"><span data-stu-id="17949-120">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="17949-121">riskScore</span><span class="sxs-lookup"><span data-stu-id="17949-121">riskScore</span></span>|<span data-ttu-id="17949-122">String</span><span class="sxs-lookup"><span data-stu-id="17949-122">String</span></span>|<span data-ttu-id="17949-123">プロバイダー生成された計算されるリスクの警告ファイルのスコアです。</span><span class="sxs-lookup"><span data-stu-id="17949-123">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="17949-124">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="17949-124">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17949-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="17949-125">JSON representation</span></span>

<span data-ttu-id="17949-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="17949-126">The following is a JSON representation of the resource.</span></span>

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
