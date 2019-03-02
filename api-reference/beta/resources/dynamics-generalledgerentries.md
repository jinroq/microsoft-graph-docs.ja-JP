---
title: 一般に、リソースの種類
description: Dynamics 365 Business Central の総勘定元帳エントリ。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0a5701451bf96773428b12b6bb715320e2ba81b5
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365760"
---
# <a name="generalledgerentries-resource-type"></a><span data-ttu-id="f5570-103">一般に、リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5570-103">generalLedgerEntries resource type</span></span>
<span data-ttu-id="f5570-104">Dynamics 365 Business Central の一般に備えた入力オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="f5570-104">Represents a generalLedgerEntry object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="f5570-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5570-105">Methods</span></span>

| <span data-ttu-id="f5570-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5570-106">Method</span></span>       | <span data-ttu-id="f5570-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f5570-107">Return Type</span></span>  |<span data-ttu-id="f5570-108">説明</span><span class="sxs-lookup"><span data-stu-id="f5570-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="f5570-109">一般に備えた gerentries エントリを取得する</span><span class="sxs-lookup"><span data-stu-id="f5570-109">Get generalLedgerEntries</span></span>](../api/dynamics-generalledgerentries-get.md)|<span data-ttu-id="f5570-110">一般に備えた gerentries</span><span class="sxs-lookup"><span data-stu-id="f5570-110">generalLedgerEntries</span></span>|<span data-ttu-id="f5570-111">G/L entry オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="f5570-111">Get a G/L entry object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f5570-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5570-112">Properties</span></span>
| <span data-ttu-id="f5570-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5570-113">Property</span></span>           | <span data-ttu-id="f5570-114">型</span><span class="sxs-lookup"><span data-stu-id="f5570-114">Type</span></span>                  |<span data-ttu-id="f5570-115">説明</span><span class="sxs-lookup"><span data-stu-id="f5570-115">Description</span></span>                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|<span data-ttu-id="f5570-116">ID</span><span class="sxs-lookup"><span data-stu-id="f5570-116">id</span></span>                  |<span data-ttu-id="f5570-117">numeric</span><span class="sxs-lookup"><span data-stu-id="f5570-117">numeric</span></span>                |<span data-ttu-id="f5570-118">G/L エントリの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="f5570-118">The unique ID of the G/L Entry.</span></span>              |
|<span data-ttu-id="f5570-119">postingdate</span><span class="sxs-lookup"><span data-stu-id="f5570-119">postingDate</span></span>         |<span data-ttu-id="f5570-120">日付</span><span class="sxs-lookup"><span data-stu-id="f5570-120">date</span></span>                   |<span data-ttu-id="f5570-121">G/L エントリの転記日を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5570-121">Specifies the posting date of the G/L Entry.</span></span> |
|<span data-ttu-id="f5570-122">documentnumber</span><span class="sxs-lookup"><span data-stu-id="f5570-122">documentNumber</span></span>      |<span data-ttu-id="f5570-123">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="f5570-123">string, maximum size 20</span></span>|<span data-ttu-id="f5570-124">G/L エントリのドキュメント番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5570-124">Specifies the document number of the G/L Entry.</span></span>|
|<span data-ttu-id="f5570-125">documentType</span><span class="sxs-lookup"><span data-stu-id="f5570-125">documentType</span></span>        |<span data-ttu-id="f5570-126">string</span><span class="sxs-lookup"><span data-stu-id="f5570-126">string</span></span>                 |<span data-ttu-id="f5570-127">G/L エントリのドキュメントの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5570-127">Specifies the document type of the G/L Entry.</span></span>|
|<span data-ttu-id="f5570-128">accountId</span><span class="sxs-lookup"><span data-stu-id="f5570-128">accountId</span></span>           |<span data-ttu-id="f5570-129">GUID</span><span class="sxs-lookup"><span data-stu-id="f5570-129">GUID</span></span>                   |<span data-ttu-id="f5570-130">G/L エントリの accountId を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5570-130">Specifies the accountId of the G/L Entry.</span></span>    |
|<span data-ttu-id="f5570-131">accountnumber</span><span class="sxs-lookup"><span data-stu-id="f5570-131">accountNumber</span></span>       |<span data-ttu-id="f5570-132">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="f5570-132">string, maximum size 20</span></span>|<span data-ttu-id="f5570-133">G/L エントリの accountnumber を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5570-133">Specifies the accountNumber of the G/L Entry.</span></span>|
|<span data-ttu-id="f5570-134">説明</span><span class="sxs-lookup"><span data-stu-id="f5570-134">description</span></span>         |<span data-ttu-id="f5570-135">文字列、最大サイズ50</span><span class="sxs-lookup"><span data-stu-id="f5570-135">string, maximum size 50</span></span>|<span data-ttu-id="f5570-136">G/L エントリの説明を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5570-136">Specifies the description of the G/L Entry.</span></span>  |
|<span data-ttu-id="f5570-137">debitamount</span><span class="sxs-lookup"><span data-stu-id="f5570-137">debitAmount</span></span>         |<span data-ttu-id="f5570-138">numeric</span><span class="sxs-lookup"><span data-stu-id="f5570-138">numeric</span></span>                |<span data-ttu-id="f5570-139">G/L エントリの金額を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5570-139">Specifies the debitAmount of the G/L Entry.</span></span>  |
|<span data-ttu-id="f5570-140">creditAmount</span><span class="sxs-lookup"><span data-stu-id="f5570-140">creditAmount</span></span>        |<span data-ttu-id="f5570-141">numeric</span><span class="sxs-lookup"><span data-stu-id="f5570-141">numeric</span></span>                |<span data-ttu-id="f5570-142">G/L エントリの creditAmount を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5570-142">Specifies the creditAmount of the G/L Entry.</span></span> |
|<span data-ttu-id="f5570-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5570-143">lastModifiedDateTime</span></span>|<span data-ttu-id="f5570-144">datetime</span><span class="sxs-lookup"><span data-stu-id="f5570-144">datetime</span></span>               |<span data-ttu-id="f5570-145">G/L エントリが変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="f5570-145">The last datetime the G/L Entry was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="f5570-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f5570-146">Relationships</span></span>
<span data-ttu-id="f5570-147">なし</span><span class="sxs-lookup"><span data-stu-id="f5570-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5570-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5570-148">JSON representation</span></span>

<span data-ttu-id="f5570-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f5570-149">Here is a JSON representation of the resource.</span></span>


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

