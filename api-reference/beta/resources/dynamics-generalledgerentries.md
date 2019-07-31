---
title: 一般に、リソースの種類
description: Dynamics 365 Business Central の総勘定元帳エントリ。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 500c78d0e29d83c68c2b7247a9787b977cc8a7b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973605"
---
# <a name="generalledgerentries-resource-type"></a><span data-ttu-id="4d0ac-103">一般に、リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4d0ac-103">generalLedgerEntries resource type</span></span>
<span data-ttu-id="4d0ac-104">Dynamics 365 Business Central の一般に備えた入力オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="4d0ac-104">Represents a generalLedgerEntry object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="4d0ac-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="4d0ac-105">Methods</span></span>

| <span data-ttu-id="4d0ac-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="4d0ac-106">Method</span></span>       | <span data-ttu-id="4d0ac-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4d0ac-107">Return Type</span></span>  |<span data-ttu-id="4d0ac-108">説明</span><span class="sxs-lookup"><span data-stu-id="4d0ac-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="4d0ac-109">一般に備えた Gerentries エントリを取得する</span><span class="sxs-lookup"><span data-stu-id="4d0ac-109">Get generalLedgerEntries</span></span>](../api/dynamics-generalledgerentries-get.md)|<span data-ttu-id="4d0ac-110">一般に備えた Gerentries</span><span class="sxs-lookup"><span data-stu-id="4d0ac-110">generalLedgerEntries</span></span>|<span data-ttu-id="4d0ac-111">G/L entry オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="4d0ac-111">Get a G/L entry object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4d0ac-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d0ac-112">Properties</span></span>
| <span data-ttu-id="4d0ac-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d0ac-113">Property</span></span>           | <span data-ttu-id="4d0ac-114">型</span><span class="sxs-lookup"><span data-stu-id="4d0ac-114">Type</span></span>                  |<span data-ttu-id="4d0ac-115">説明</span><span class="sxs-lookup"><span data-stu-id="4d0ac-115">Description</span></span>                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|<span data-ttu-id="4d0ac-116">id</span><span class="sxs-lookup"><span data-stu-id="4d0ac-116">id</span></span>                  |<span data-ttu-id="4d0ac-117">数値</span><span class="sxs-lookup"><span data-stu-id="4d0ac-117">numeric</span></span>                |<span data-ttu-id="4d0ac-118">G/L エントリの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="4d0ac-118">The unique ID of the G/L Entry.</span></span>              |
|<span data-ttu-id="4d0ac-119">postingDate</span><span class="sxs-lookup"><span data-stu-id="4d0ac-119">postingDate</span></span>         |<span data-ttu-id="4d0ac-120">date</span><span class="sxs-lookup"><span data-stu-id="4d0ac-120">date</span></span>                   |<span data-ttu-id="4d0ac-121">G/L エントリの転記日を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d0ac-121">Specifies the posting date of the G/L Entry.</span></span> |
|<span data-ttu-id="4d0ac-122">documentNumber</span><span class="sxs-lookup"><span data-stu-id="4d0ac-122">documentNumber</span></span>      |<span data-ttu-id="4d0ac-123">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="4d0ac-123">string, maximum size 20</span></span>|<span data-ttu-id="4d0ac-124">G/L エントリのドキュメント番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d0ac-124">Specifies the document number of the G/L Entry.</span></span>|
|<span data-ttu-id="4d0ac-125">documentType</span><span class="sxs-lookup"><span data-stu-id="4d0ac-125">documentType</span></span>        |<span data-ttu-id="4d0ac-126">string</span><span class="sxs-lookup"><span data-stu-id="4d0ac-126">string</span></span>                 |<span data-ttu-id="4d0ac-127">G/L エントリのドキュメントの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d0ac-127">Specifies the document type of the G/L Entry.</span></span>|
|<span data-ttu-id="4d0ac-128">accountId</span><span class="sxs-lookup"><span data-stu-id="4d0ac-128">accountId</span></span>           |<span data-ttu-id="4d0ac-129">GUID</span><span class="sxs-lookup"><span data-stu-id="4d0ac-129">GUID</span></span>                   |<span data-ttu-id="4d0ac-130">G/L エントリの accountId を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d0ac-130">Specifies the accountId of the G/L Entry.</span></span>    |
|<span data-ttu-id="4d0ac-131">accountNumber</span><span class="sxs-lookup"><span data-stu-id="4d0ac-131">accountNumber</span></span>       |<span data-ttu-id="4d0ac-132">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="4d0ac-132">string, maximum size 20</span></span>|<span data-ttu-id="4d0ac-133">G/L エントリの accountNumber を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d0ac-133">Specifies the accountNumber of the G/L Entry.</span></span>|
|<span data-ttu-id="4d0ac-134">description</span><span class="sxs-lookup"><span data-stu-id="4d0ac-134">description</span></span>         |<span data-ttu-id="4d0ac-135">文字列、最大サイズ50</span><span class="sxs-lookup"><span data-stu-id="4d0ac-135">string, maximum size 50</span></span>|<span data-ttu-id="4d0ac-136">G/L エントリの説明を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d0ac-136">Specifies the description of the G/L Entry.</span></span>  |
|<span data-ttu-id="4d0ac-137">debitAmount</span><span class="sxs-lookup"><span data-stu-id="4d0ac-137">debitAmount</span></span>         |<span data-ttu-id="4d0ac-138">数値</span><span class="sxs-lookup"><span data-stu-id="4d0ac-138">numeric</span></span>                |<span data-ttu-id="4d0ac-139">G/L エントリの金額を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d0ac-139">Specifies the debitAmount of the G/L Entry.</span></span>  |
|<span data-ttu-id="4d0ac-140">creditAmount</span><span class="sxs-lookup"><span data-stu-id="4d0ac-140">creditAmount</span></span>        |<span data-ttu-id="4d0ac-141">数値</span><span class="sxs-lookup"><span data-stu-id="4d0ac-141">numeric</span></span>                |<span data-ttu-id="4d0ac-142">G/L エントリの creditAmount を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d0ac-142">Specifies the creditAmount of the G/L Entry.</span></span> |
|<span data-ttu-id="4d0ac-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d0ac-143">lastModifiedDateTime</span></span>|<span data-ttu-id="4d0ac-144">datetime</span><span class="sxs-lookup"><span data-stu-id="4d0ac-144">datetime</span></span>               |<span data-ttu-id="4d0ac-145">G/L エントリが変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="4d0ac-145">The last datetime the G/L Entry was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="4d0ac-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4d0ac-146">Relationships</span></span>
<span data-ttu-id="4d0ac-147">なし</span><span class="sxs-lookup"><span data-stu-id="4d0ac-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d0ac-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4d0ac-148">JSON representation</span></span>

<span data-ttu-id="4d0ac-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4d0ac-149">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "int",
  "postingDate": "Date",
  "documentNumber": "string",
  "documentType": "string",
  "accountId": "GUID",
  "accountNumber": "string",
  "description": "string",
  "debitAmount": "decimal",
  "creditAmount": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

