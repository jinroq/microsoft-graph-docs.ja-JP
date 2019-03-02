---
title: 顧客の支払いリソースの種類
description: Dynamics 365 Business Central の顧客の支払いオブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 9063a9066c51956596e4f0aa918a2e7a53bf2ab9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365613"
---
# <a name="customerpayments-resource-type"></a><span data-ttu-id="a3e1c-103">顧客の支払いリソースの種類</span><span class="sxs-lookup"><span data-stu-id="a3e1c-103">customerPayments resource type</span></span>
<span data-ttu-id="a3e1c-104">Dynamics 365 Business Central の顧客の支払いを表します。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-104">Represents a customer payment in Dynamics 365 Business Central.</span></span> <span data-ttu-id="a3e1c-105">顧客支払は、顧客の支払仕訳帳に明細行として入力されます。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-105">A customer payment is entered as a line in a customer payment journal.</span></span>

## <a name="methods"></a><span data-ttu-id="a3e1c-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a3e1c-106">Methods</span></span>

| <span data-ttu-id="a3e1c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a3e1c-107">Method</span></span>         | <span data-ttu-id="a3e1c-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a3e1c-108">Return Type</span></span>  |<span data-ttu-id="a3e1c-109">説明</span><span class="sxs-lookup"><span data-stu-id="a3e1c-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="a3e1c-110">顧客の支払いを取得する</span><span class="sxs-lookup"><span data-stu-id="a3e1c-110">Get customerPayments</span></span>](../api/dynamics-customerpayment-get.md)|<span data-ttu-id="a3e1c-111">顧客の支払い</span><span class="sxs-lookup"><span data-stu-id="a3e1c-111">customerPayments</span></span>|<span data-ttu-id="a3e1c-112">顧客支払を取得します。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-112">Gets a customer payment.</span></span>|
|[<span data-ttu-id="a3e1c-113">顧客の支払いを投稿する</span><span class="sxs-lookup"><span data-stu-id="a3e1c-113">Post customerPayments</span></span>](../api/dynamics-create-customerpayment.md)|<span data-ttu-id="a3e1c-114">顧客の支払い</span><span class="sxs-lookup"><span data-stu-id="a3e1c-114">customerPayments</span></span>|<span data-ttu-id="a3e1c-115">顧客の支払いを作成します。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-115">Creates a customer payment.</span></span>|
|[<span data-ttu-id="a3e1c-116">更新プログラムの顧客の支払い</span><span class="sxs-lookup"><span data-stu-id="a3e1c-116">Patch customerPayments</span></span>](../api/dynamics-customerpayment-update.md)|<span data-ttu-id="a3e1c-117">顧客の支払い</span><span class="sxs-lookup"><span data-stu-id="a3e1c-117">customerPayments</span></span>|<span data-ttu-id="a3e1c-118">顧客の支払いを更新します。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-118">Updates a customer payment.</span></span>|
|[<span data-ttu-id="a3e1c-119">顧客の支払いを削除する</span><span class="sxs-lookup"><span data-stu-id="a3e1c-119">Delete customerPayments</span></span>](../api/dynamics-customerpayment-delete.md)|<span data-ttu-id="a3e1c-120">none</span><span class="sxs-lookup"><span data-stu-id="a3e1c-120">none</span></span>|<span data-ttu-id="a3e1c-121">顧客の支払を削除します。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-121">Deletes a customer payment.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3e1c-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3e1c-122">Properties</span></span>
| <span data-ttu-id="a3e1c-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3e1c-123">Property</span></span>     | <span data-ttu-id="a3e1c-124">型</span><span class="sxs-lookup"><span data-stu-id="a3e1c-124">Type</span></span>    |<span data-ttu-id="a3e1c-125">説明</span><span class="sxs-lookup"><span data-stu-id="a3e1c-125">Description</span></span>|
|:-------------|:--------|:----------|
|<span data-ttu-id="a3e1c-126">ID</span><span class="sxs-lookup"><span data-stu-id="a3e1c-126">id</span></span>|<span data-ttu-id="a3e1c-127">GUID</span><span class="sxs-lookup"><span data-stu-id="a3e1c-127">GUID</span></span>|<span data-ttu-id="a3e1c-128">顧客の支払の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-128">The unique ID of the customer payment.</span></span> <span data-ttu-id="a3e1c-129">編集不可。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-129">Non-editable.</span></span>|
|<span data-ttu-id="a3e1c-130">journalDisplayName</span><span class="sxs-lookup"><span data-stu-id="a3e1c-130">journalDisplayName</span></span>|<span data-ttu-id="a3e1c-131">string</span><span class="sxs-lookup"><span data-stu-id="a3e1c-131">string</span></span>|<span data-ttu-id="a3e1c-132">支払いレコードが行である顧客支払仕訳帳。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-132">The customer payment journal in which the payment record is a line.</span></span>|
|<span data-ttu-id="a3e1c-133">lineNumber</span><span class="sxs-lookup"><span data-stu-id="a3e1c-133">lineNumber</span></span>|<span data-ttu-id="a3e1c-134">integer</span><span class="sxs-lookup"><span data-stu-id="a3e1c-134">integer</span></span>|<span data-ttu-id="a3e1c-135">顧客の支払回数。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-135">The number of the customer payment.</span></span>|
|<span data-ttu-id="a3e1c-136">customerId</span><span class="sxs-lookup"><span data-stu-id="a3e1c-136">customerId</span></span>|<span data-ttu-id="a3e1c-137">GUID</span><span class="sxs-lookup"><span data-stu-id="a3e1c-137">GUID</span></span>|<span data-ttu-id="a3e1c-138">支払いが関連付けられている顧客の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-138">The unique ID of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="a3e1c-139">顧客番号</span><span class="sxs-lookup"><span data-stu-id="a3e1c-139">customerNumber</span></span>|<span data-ttu-id="a3e1c-140">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="a3e1c-140">string, maximum size 20</span></span>|<span data-ttu-id="a3e1c-141">支払いが関連付けられている顧客の番号。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-141">The number of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="a3e1c-142">contactId</span><span class="sxs-lookup"><span data-stu-id="a3e1c-142">contactId</span></span>|<span data-ttu-id="a3e1c-143">文字列、最大サイズ250</span><span class="sxs-lookup"><span data-stu-id="a3e1c-143">string, maximum size 250</span></span>|<span data-ttu-id="a3e1c-144">指定された顧客の exchange 連絡先 id。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-144">The exchange contact id for the given customer.</span></span> <span data-ttu-id="a3e1c-145">顧客 id が指定されていない場合は、連絡先 id を使用して検索します。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-145">If a customer id is not specified, we will use the contact id to find it.</span></span>|
|<span data-ttu-id="a3e1c-146">postingdate</span><span class="sxs-lookup"><span data-stu-id="a3e1c-146">postingDate</span></span>|<span data-ttu-id="a3e1c-147">日付</span><span class="sxs-lookup"><span data-stu-id="a3e1c-147">date</span></span>|<span data-ttu-id="a3e1c-148">顧客の支払が転記される日付。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-148">The date that the customer payment is posted.</span></span>|
|<span data-ttu-id="a3e1c-149">documentnumber</span><span class="sxs-lookup"><span data-stu-id="a3e1c-149">documentNumber</span></span>|<span data-ttu-id="a3e1c-150">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="a3e1c-150">string, maximum size 20</span></span>|<span data-ttu-id="a3e1c-151">顧客支払のドキュメント番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-151">Specifies a document number for the customer payment.</span></span>|
|<span data-ttu-id="a3e1c-152">externaldocumentnumber</span><span class="sxs-lookup"><span data-stu-id="a3e1c-152">externalDocumentNumber</span></span>|<span data-ttu-id="a3e1c-153">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="a3e1c-153">string, maximum size 20</span></span>|<span data-ttu-id="a3e1c-154">顧客支払の外部ドキュメント番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-154">Specifies an external document number for the customer payment.</span></span>|
|<span data-ttu-id="a3e1c-155">値</span><span class="sxs-lookup"><span data-stu-id="a3e1c-155">amount</span></span>|<span data-ttu-id="a3e1c-156">decimal</span><span class="sxs-lookup"><span data-stu-id="a3e1c-156">decimal</span></span>|<span data-ttu-id="a3e1c-157">顧客の支払を構成する合計金額 (VAT を含む) を指定します。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-157">Specifies the total amount (including VAT) that the customer payment consists of.</span></span>|
|<span data-ttu-id="a3e1c-158">appliesToInvoiceId</span><span class="sxs-lookup"><span data-stu-id="a3e1c-158">appliesToInvoiceId</span></span>|<span data-ttu-id="a3e1c-159">GUID</span><span class="sxs-lookup"><span data-stu-id="a3e1c-159">GUID</span></span>|<span data-ttu-id="a3e1c-160">支払が関連付けられている請求書の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-160">The unique ID of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="a3e1c-161">appliesToInvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="a3e1c-161">appliesToInvoiceNumber</span></span>|<span data-ttu-id="a3e1c-162">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="a3e1c-162">string, maximum size 20</span></span>|<span data-ttu-id="a3e1c-163">支払が関連付けられている請求書の番号。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-163">The number of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="a3e1c-164">説明</span><span class="sxs-lookup"><span data-stu-id="a3e1c-164">description</span></span>|<span data-ttu-id="a3e1c-165">文字列、最大サイズ50</span><span class="sxs-lookup"><span data-stu-id="a3e1c-165">string, maximum size 50</span></span>|<span data-ttu-id="a3e1c-166">ユーザーまたは autocreated によって提供される顧客の支払いの説明。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-166">The description of the customer payment, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="a3e1c-167">コメント</span><span class="sxs-lookup"><span data-stu-id="a3e1c-167">comment</span></span>|<span data-ttu-id="a3e1c-168">文字列、最大サイズ250</span><span class="sxs-lookup"><span data-stu-id="a3e1c-168">string, maximum size 250</span></span>|<span data-ttu-id="a3e1c-169">顧客支払に対してユーザーが指定したコメント。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-169">A user specified comment on the customer payment.</span></span>|
|<span data-ttu-id="a3e1c-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3e1c-170">lastModifiedDateTime</span></span>|<span data-ttu-id="a3e1c-171">datetime</span><span class="sxs-lookup"><span data-stu-id="a3e1c-171">datetime</span></span>|<span data-ttu-id="a3e1c-172">顧客の支払が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-172">The last datetime the customer payment was modified.</span></span> <span data-ttu-id="a3e1c-173">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-173">Read-Only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="a3e1c-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a3e1c-174">Relationships</span></span>
<span data-ttu-id="a3e1c-175">顧客支払は、顧客の支払仕訳帳のサブページです。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-175">A customer payment is a subpage of a customer payment journal.</span></span> <span data-ttu-id="a3e1c-176">直接アクセスすることはできません。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-176">It cannot be accessed directly.</span></span>

<span data-ttu-id="a3e1c-177">顧客支払は、寸法線の "親エンティティ" にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-177">A customer payment can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="a3e1c-178">Customers テーブルに Customer (customerId) が存在している必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-178">A Customer (customerId) must exist in the Customers table.</span></span>

<span data-ttu-id="a3e1c-179">請求書 (appliesToInvoiceId) は、[売上請求書] テーブルに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-179">An Invoice (appliesToInvoiceId) must exist in the Sales Invoices Table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a3e1c-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a3e1c-180">JSON representation</span></span>

<span data-ttu-id="a3e1c-181">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a3e1c-181">Here is a JSON representation of the resource.</span></span>

```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "customerId": "GUID",
    "customerNumber": "string",
    "contactId": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "appliesToInvoiceId": "GUID",
    "appliesToInvoiceNumber": "string",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```

