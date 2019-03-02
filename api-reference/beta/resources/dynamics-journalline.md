---
title: journalLines リソースの種類
description: Dynamics 365 Business Central のジャーナル明細行。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 7a6841bcc2f893f8ca794e7d8e6aeafbcd4e48ca
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365956"
---
# <a name="journallines-resource-type"></a><span data-ttu-id="a4575-103">journalLines リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4575-103">journalLines resource type</span></span>
<span data-ttu-id="a4575-104">Dynamics 365 Business Central のジャーナルの行を表します。</span><span class="sxs-lookup"><span data-stu-id="a4575-104">Represents a line in a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="a4575-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4575-105">Methods</span></span>

| <span data-ttu-id="a4575-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4575-106">Method</span></span>                                                    | <span data-ttu-id="a4575-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a4575-107">Return Type</span></span>|<span data-ttu-id="a4575-108">説明</span><span class="sxs-lookup"><span data-stu-id="a4575-108">Description</span></span>         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[<span data-ttu-id="a4575-109">journalLines を取得する</span><span class="sxs-lookup"><span data-stu-id="a4575-109">Get journalLines</span></span>](../api/dynamics-journalline-get.md)      |<span data-ttu-id="a4575-110">journalLines</span><span class="sxs-lookup"><span data-stu-id="a4575-110">journalLines</span></span>|<span data-ttu-id="a4575-111">仕訳帳明細行を取得します。</span><span class="sxs-lookup"><span data-stu-id="a4575-111">Gets a journal line.</span></span>   |
|[<span data-ttu-id="a4575-112">Post journalLines</span><span class="sxs-lookup"><span data-stu-id="a4575-112">Post journalLines</span></span>](../api/dynamics-create-journalline.md)  |<span data-ttu-id="a4575-113">journalLines</span><span class="sxs-lookup"><span data-stu-id="a4575-113">journalLines</span></span>|<span data-ttu-id="a4575-114">仕訳帳明細行を作成します。</span><span class="sxs-lookup"><span data-stu-id="a4575-114">Creates a journal line.</span></span>|
|[<span data-ttu-id="a4575-115">Patch journalLines</span><span class="sxs-lookup"><span data-stu-id="a4575-115">Patch journalLines</span></span>](../api/dynamics-journalline-update.md) |<span data-ttu-id="a4575-116">journalLines</span><span class="sxs-lookup"><span data-stu-id="a4575-116">journalLines</span></span>|<span data-ttu-id="a4575-117">仕訳帳明細行を更新します。</span><span class="sxs-lookup"><span data-stu-id="a4575-117">Updates a journal line.</span></span>|
|[<span data-ttu-id="a4575-118">journalLines の削除</span><span class="sxs-lookup"><span data-stu-id="a4575-118">Delete journalLines</span></span>](../api/dynamics-journalline-delete.md)|<span data-ttu-id="a4575-119">none</span><span class="sxs-lookup"><span data-stu-id="a4575-119">none</span></span>        |<span data-ttu-id="a4575-120">仕訳帳明細行を削除します。</span><span class="sxs-lookup"><span data-stu-id="a4575-120">Deletes a journal line.</span></span>|

## <a name="properties"></a><span data-ttu-id="a4575-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4575-121">Properties</span></span>
| <span data-ttu-id="a4575-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4575-122">Property</span></span>             | <span data-ttu-id="a4575-123">型</span><span class="sxs-lookup"><span data-stu-id="a4575-123">Type</span></span>                   |<span data-ttu-id="a4575-124">説明</span><span class="sxs-lookup"><span data-stu-id="a4575-124">Description</span></span>                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|<span data-ttu-id="a4575-125">ID</span><span class="sxs-lookup"><span data-stu-id="a4575-125">id</span></span>                    |<span data-ttu-id="a4575-126">GUID</span><span class="sxs-lookup"><span data-stu-id="a4575-126">GUID</span></span>                    |<span data-ttu-id="a4575-127">仕訳帳明細行の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="a4575-127">The unique ID of the journal line.</span></span> <span data-ttu-id="a4575-128">編集不可。</span><span class="sxs-lookup"><span data-stu-id="a4575-128">Non-editable.</span></span>                   |
|<span data-ttu-id="a4575-129">journalDisplayName</span><span class="sxs-lookup"><span data-stu-id="a4575-129">journalDisplayName</span></span>    |<span data-ttu-id="a4575-130">文字列、最大サイズ10</span><span class="sxs-lookup"><span data-stu-id="a4575-130">string, maximum size 10</span></span> |<span data-ttu-id="a4575-131">この行が属するジャーナルの表示名。</span><span class="sxs-lookup"><span data-stu-id="a4575-131">The display name of the journal that this line belongs to.</span></span> <span data-ttu-id="a4575-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a4575-132">Read-Only.</span></span>|
|<span data-ttu-id="a4575-133">lineNumber</span><span class="sxs-lookup"><span data-stu-id="a4575-133">lineNumber</span></span>            |<span data-ttu-id="a4575-134">integer</span><span class="sxs-lookup"><span data-stu-id="a4575-134">integer</span></span>                 |<span data-ttu-id="a4575-135">仕訳帳明細行の番号。</span><span class="sxs-lookup"><span data-stu-id="a4575-135">The number of the journal line.</span></span>                                    |
|<span data-ttu-id="a4575-136">accountId</span><span class="sxs-lookup"><span data-stu-id="a4575-136">accountId</span></span>             |<span data-ttu-id="a4575-137">GUID</span><span class="sxs-lookup"><span data-stu-id="a4575-137">GUID</span></span>                    |<span data-ttu-id="a4575-138">仕訳帳明細行が関連付けられているアカウントの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="a4575-138">The unique ID of the account that the journal line is related to.</span></span>  |
|<span data-ttu-id="a4575-139">accountnumber</span><span class="sxs-lookup"><span data-stu-id="a4575-139">accountNumber</span></span>         |<span data-ttu-id="a4575-140">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="a4575-140">string, maximum size 20</span></span> |<span data-ttu-id="a4575-141">仕訳帳明細行が関連付けられているアカウントの番号。</span><span class="sxs-lookup"><span data-stu-id="a4575-141">The number of the account that the journal line is related to.</span></span>     |
|<span data-ttu-id="a4575-142">postingdate</span><span class="sxs-lookup"><span data-stu-id="a4575-142">postingDate</span></span>           |<span data-ttu-id="a4575-143">日付</span><span class="sxs-lookup"><span data-stu-id="a4575-143">date</span></span>                    |<span data-ttu-id="a4575-144">仕訳帳明細行が転記される日付。</span><span class="sxs-lookup"><span data-stu-id="a4575-144">The date that the journal line is posted.</span></span>                          |
|<span data-ttu-id="a4575-145">documentnumber</span><span class="sxs-lookup"><span data-stu-id="a4575-145">documentNumber</span></span>        |<span data-ttu-id="a4575-146">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="a4575-146">string, maximum size 20</span></span> |<span data-ttu-id="a4575-147">仕訳帳明細行の文書番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4575-147">Specifies a document number for the journal line.</span></span>                  |
|<span data-ttu-id="a4575-148">externaldocumentnumber</span><span class="sxs-lookup"><span data-stu-id="a4575-148">externalDocumentNumber</span></span>|<span data-ttu-id="a4575-149">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="a4575-149">string, maximum size 20</span></span> |<span data-ttu-id="a4575-150">仕訳帳明細行の外部ドキュメント番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4575-150">Specifies an external document number for the journal line.</span></span>        |
|<span data-ttu-id="a4575-151">値</span><span class="sxs-lookup"><span data-stu-id="a4575-151">amount</span></span>                |<span data-ttu-id="a4575-152">decimal</span><span class="sxs-lookup"><span data-stu-id="a4575-152">decimal</span></span>                 |<span data-ttu-id="a4575-153">仕訳帳明細行を構成する合計金額 (VAT を含む) を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4575-153">Specifies the total amount (including VAT) that the journal line consists of.</span></span>|
|<span data-ttu-id="a4575-154">説明</span><span class="sxs-lookup"><span data-stu-id="a4575-154">description</span></span>           |<span data-ttu-id="a4575-155">文字列、最大サイズ50</span><span class="sxs-lookup"><span data-stu-id="a4575-155">string, maximum size 50</span></span> |<span data-ttu-id="a4575-156">ユーザーまたは autocreated によって提供される、仕訳帳明細行の説明。</span><span class="sxs-lookup"><span data-stu-id="a4575-156">The description of the journal line, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="a4575-157">コメント</span><span class="sxs-lookup"><span data-stu-id="a4575-157">comment</span></span>               |<span data-ttu-id="a4575-158">文字列、最大サイズ250</span><span class="sxs-lookup"><span data-stu-id="a4575-158">string, maximum size 250</span></span>|<span data-ttu-id="a4575-159">ユーザーが仕訳帳明細行に対して指定したコメント。</span><span class="sxs-lookup"><span data-stu-id="a4575-159">A user specified comment on the journal line.</span></span>                      |
|<span data-ttu-id="a4575-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4575-160">lastModifiedDateTime</span></span>  |<span data-ttu-id="a4575-161">datetime</span><span class="sxs-lookup"><span data-stu-id="a4575-161">datetime</span></span>                |<span data-ttu-id="a4575-162">履歴明細行が変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="a4575-162">The last datetime the journal line was modified.</span></span> <span data-ttu-id="a4575-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a4575-163">Read-Only.</span></span>        |

## <a name="relationships"></a><span data-ttu-id="a4575-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a4575-164">Relationships</span></span>
<span data-ttu-id="a4575-165">ジャーナル明細行は、ジャーナルのサブページです。</span><span class="sxs-lookup"><span data-stu-id="a4575-165">A journal line is a subpage of a journal.</span></span> <span data-ttu-id="a4575-166">直接アクセスすることはできません。</span><span class="sxs-lookup"><span data-stu-id="a4575-166">It cannot be accessed directly.</span></span>

<span data-ttu-id="a4575-167">仕訳線は、寸法線の "親エンティティ" にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a4575-167">A journal line can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="a4575-168">アカウント (accountId) は、Accounts テーブルに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4575-168">An Account (accountId) must exist in the Accounts table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a4575-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4575-169">JSON representation</span></span>

<span data-ttu-id="a4575-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a4575-170">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "accountId": "GUID",
    "accountNumber": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```
