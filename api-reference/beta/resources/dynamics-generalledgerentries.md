---
title: 一般に、リソースの種類
description: Dynamics 365 Business Central の総勘定元帳エントリ。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0a5701451bf96773428b12b6bb715320e2ba81b5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507240"
---
# <a name="generalledgerentries-resource-type"></a><span data-ttu-id="09d1b-103">一般に、リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09d1b-103">generalLedgerEntries resource type</span></span>
<span data-ttu-id="09d1b-104">Dynamics 365 Business Central の一般に備えた入力オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="09d1b-104">Represents a generalLedgerEntry object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="09d1b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="09d1b-105">Methods</span></span>

| <span data-ttu-id="09d1b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="09d1b-106">Method</span></span>       | <span data-ttu-id="09d1b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="09d1b-107">Return Type</span></span>  |<span data-ttu-id="09d1b-108">説明</span><span class="sxs-lookup"><span data-stu-id="09d1b-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="09d1b-109">一般に備えた gerentries エントリを取得する</span><span class="sxs-lookup"><span data-stu-id="09d1b-109">Get generalLedgerEntries</span></span>](../api/dynamics-generalledgerentries-get.md)|<span data-ttu-id="09d1b-110">一般に備えた gerentries</span><span class="sxs-lookup"><span data-stu-id="09d1b-110">generalLedgerEntries</span></span>|<span data-ttu-id="09d1b-111">G/L entry オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="09d1b-111">Get a G/L entry object.</span></span>|

## <a name="properties"></a><span data-ttu-id="09d1b-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09d1b-112">Properties</span></span>
| <span data-ttu-id="09d1b-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09d1b-113">Property</span></span>           | <span data-ttu-id="09d1b-114">型</span><span class="sxs-lookup"><span data-stu-id="09d1b-114">Type</span></span>                  |<span data-ttu-id="09d1b-115">説明</span><span class="sxs-lookup"><span data-stu-id="09d1b-115">Description</span></span>                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|<span data-ttu-id="09d1b-116">id</span><span class="sxs-lookup"><span data-stu-id="09d1b-116">id</span></span>                  |<span data-ttu-id="09d1b-117">数値</span><span class="sxs-lookup"><span data-stu-id="09d1b-117">numeric</span></span>                |<span data-ttu-id="09d1b-118">G/L エントリの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="09d1b-118">The unique ID of the G/L Entry.</span></span>              |
|<span data-ttu-id="09d1b-119">postingdate</span><span class="sxs-lookup"><span data-stu-id="09d1b-119">postingDate</span></span>         |<span data-ttu-id="09d1b-120">日付</span><span class="sxs-lookup"><span data-stu-id="09d1b-120">date</span></span>                   |<span data-ttu-id="09d1b-121">G/L エントリの転記日を指定します。</span><span class="sxs-lookup"><span data-stu-id="09d1b-121">Specifies the posting date of the G/L Entry.</span></span> |
|<span data-ttu-id="09d1b-122">documentnumber</span><span class="sxs-lookup"><span data-stu-id="09d1b-122">documentNumber</span></span>      |<span data-ttu-id="09d1b-123">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="09d1b-123">string, maximum size 20</span></span>|<span data-ttu-id="09d1b-124">G/L エントリのドキュメント番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="09d1b-124">Specifies the document number of the G/L Entry.</span></span>|
|<span data-ttu-id="09d1b-125">documentType</span><span class="sxs-lookup"><span data-stu-id="09d1b-125">documentType</span></span>        |<span data-ttu-id="09d1b-126">string</span><span class="sxs-lookup"><span data-stu-id="09d1b-126">string</span></span>                 |<span data-ttu-id="09d1b-127">G/L エントリのドキュメントの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="09d1b-127">Specifies the document type of the G/L Entry.</span></span>|
|<span data-ttu-id="09d1b-128">accountId</span><span class="sxs-lookup"><span data-stu-id="09d1b-128">accountId</span></span>           |<span data-ttu-id="09d1b-129">GUID</span><span class="sxs-lookup"><span data-stu-id="09d1b-129">GUID</span></span>                   |<span data-ttu-id="09d1b-130">G/L エントリの accountId を指定します。</span><span class="sxs-lookup"><span data-stu-id="09d1b-130">Specifies the accountId of the G/L Entry.</span></span>    |
|<span data-ttu-id="09d1b-131">accountnumber</span><span class="sxs-lookup"><span data-stu-id="09d1b-131">accountNumber</span></span>       |<span data-ttu-id="09d1b-132">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="09d1b-132">string, maximum size 20</span></span>|<span data-ttu-id="09d1b-133">G/L エントリの accountnumber を指定します。</span><span class="sxs-lookup"><span data-stu-id="09d1b-133">Specifies the accountNumber of the G/L Entry.</span></span>|
|<span data-ttu-id="09d1b-134">説明</span><span class="sxs-lookup"><span data-stu-id="09d1b-134">description</span></span>         |<span data-ttu-id="09d1b-135">文字列、最大サイズ50</span><span class="sxs-lookup"><span data-stu-id="09d1b-135">string, maximum size 50</span></span>|<span data-ttu-id="09d1b-136">G/L エントリの説明を指定します。</span><span class="sxs-lookup"><span data-stu-id="09d1b-136">Specifies the description of the G/L Entry.</span></span>  |
|<span data-ttu-id="09d1b-137">debitamount</span><span class="sxs-lookup"><span data-stu-id="09d1b-137">debitAmount</span></span>         |<span data-ttu-id="09d1b-138">数値</span><span class="sxs-lookup"><span data-stu-id="09d1b-138">numeric</span></span>                |<span data-ttu-id="09d1b-139">G/L エントリの金額を指定します。</span><span class="sxs-lookup"><span data-stu-id="09d1b-139">Specifies the debitAmount of the G/L Entry.</span></span>  |
|<span data-ttu-id="09d1b-140">creditAmount</span><span class="sxs-lookup"><span data-stu-id="09d1b-140">creditAmount</span></span>        |<span data-ttu-id="09d1b-141">数値</span><span class="sxs-lookup"><span data-stu-id="09d1b-141">numeric</span></span>                |<span data-ttu-id="09d1b-142">G/L エントリの creditAmount を指定します。</span><span class="sxs-lookup"><span data-stu-id="09d1b-142">Specifies the creditAmount of the G/L Entry.</span></span> |
|<span data-ttu-id="09d1b-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09d1b-143">lastModifiedDateTime</span></span>|<span data-ttu-id="09d1b-144">datetime</span><span class="sxs-lookup"><span data-stu-id="09d1b-144">datetime</span></span>               |<span data-ttu-id="09d1b-145">G/L エントリが変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="09d1b-145">The last datetime the G/L Entry was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="09d1b-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09d1b-146">Relationships</span></span>
<span data-ttu-id="09d1b-147">なし</span><span class="sxs-lookup"><span data-stu-id="09d1b-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09d1b-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09d1b-148">JSON representation</span></span>

<span data-ttu-id="09d1b-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09d1b-149">Here is a JSON representation of the resource.</span></span>


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

