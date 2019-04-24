---
title: customers リソースの種類
description: Dynamics 365 Business Central の顧客を表します。
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e4daa28018001fb6cb6e4866bedf8e256a72abef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507260"
---
# <a name="customers-resource-type"></a><span data-ttu-id="3ac20-103">customers リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3ac20-103">customers resource type</span></span>
<span data-ttu-id="3ac20-104">Dynamics 365 Business Central の顧客を表します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-104">Represents a customer in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="3ac20-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="3ac20-105">Methods</span></span>

| <span data-ttu-id="3ac20-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="3ac20-106">Method</span></span>                                              |<span data-ttu-id="3ac20-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3ac20-107">Return Type</span></span>| <span data-ttu-id="3ac20-108">説明</span><span class="sxs-lookup"><span data-stu-id="3ac20-108">Description</span></span>      |
|:----------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="3ac20-109">顧客を取得する</span><span class="sxs-lookup"><span data-stu-id="3ac20-109">Get customers</span></span>](../api/dynamics-customer-get.md)      |<span data-ttu-id="3ac20-110">ユーザー</span><span class="sxs-lookup"><span data-stu-id="3ac20-110">customers</span></span>   |<span data-ttu-id="3ac20-111">顧客を取得します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-111">Gets a customer.</span></span>   |
|[<span data-ttu-id="3ac20-112">顧客を作成する</span><span class="sxs-lookup"><span data-stu-id="3ac20-112">Create customers</span></span>](../api/dynamics-create-customer.md)|<span data-ttu-id="3ac20-113">ユーザー</span><span class="sxs-lookup"><span data-stu-id="3ac20-113">customers</span></span>   |<span data-ttu-id="3ac20-114">顧客を作成します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-114">Creates a customer.</span></span>|
|[<span data-ttu-id="3ac20-115">顧客を更新する</span><span class="sxs-lookup"><span data-stu-id="3ac20-115">Update customers</span></span>](../api/dynamics-customer-update.md)|<span data-ttu-id="3ac20-116">ユーザー</span><span class="sxs-lookup"><span data-stu-id="3ac20-116">customers</span></span>   |<span data-ttu-id="3ac20-117">顧客を更新します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-117">Updates a customer.</span></span>|
|[<span data-ttu-id="3ac20-118">顧客を削除する</span><span class="sxs-lookup"><span data-stu-id="3ac20-118">Delete customers</span></span>](../api/dynamics-customer-delete.md)|<span data-ttu-id="3ac20-119">なし</span><span class="sxs-lookup"><span data-stu-id="3ac20-119">none</span></span>        |<span data-ttu-id="3ac20-120">顧客を削除します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-120">Deletes a customer.</span></span>|

## <a name="properties"></a><span data-ttu-id="3ac20-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ac20-121">Properties</span></span>
| <span data-ttu-id="3ac20-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ac20-122">Property</span></span>    | <span data-ttu-id="3ac20-123">型</span><span class="sxs-lookup"><span data-stu-id="3ac20-123">Type</span></span>     |<span data-ttu-id="3ac20-124">説明</span><span class="sxs-lookup"><span data-stu-id="3ac20-124">Description</span></span>|
|:------------|:---------|:----------|
|<span data-ttu-id="3ac20-125">id</span><span class="sxs-lookup"><span data-stu-id="3ac20-125">id</span></span>           |<span data-ttu-id="3ac20-126">GUID</span><span class="sxs-lookup"><span data-stu-id="3ac20-126">GUID</span></span>      |<span data-ttu-id="3ac20-127">アイテムの一意の ID です。</span><span class="sxs-lookup"><span data-stu-id="3ac20-127">The unique ID of the item.</span></span> <span data-ttu-id="3ac20-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="3ac20-128">Non-editable.</span></span>|
|<span data-ttu-id="3ac20-129">number</span><span class="sxs-lookup"><span data-stu-id="3ac20-129">number</span></span>       |<span data-ttu-id="3ac20-130">string</span><span class="sxs-lookup"><span data-stu-id="3ac20-130">string</span></span>    |<span data-ttu-id="3ac20-131">顧客番号。</span><span class="sxs-lookup"><span data-stu-id="3ac20-131">The customer number.</span></span>|
|<span data-ttu-id="3ac20-132">displayName</span><span class="sxs-lookup"><span data-stu-id="3ac20-132">displayName</span></span>  |<span data-ttu-id="3ac20-133">string</span><span class="sxs-lookup"><span data-stu-id="3ac20-133">string</span></span>    |<span data-ttu-id="3ac20-134">顧客の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-134">Specifies the customer's name.</span></span> <span data-ttu-id="3ac20-135">この名前は、顧客のすべての販売ドキュメントに表示されます。</span><span class="sxs-lookup"><span data-stu-id="3ac20-135">This name will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="3ac20-136">type</span><span class="sxs-lookup"><span data-stu-id="3ac20-136">type</span></span>         |<span data-ttu-id="3ac20-137">string</span><span class="sxs-lookup"><span data-stu-id="3ac20-137">string</span></span>    |<span data-ttu-id="3ac20-138">顧客の種類として、"Company" または "Person" を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-138">Specifies the type of customer, can be "Company" or "Person".</span></span>|
|<span data-ttu-id="3ac20-139">address</span><span class="sxs-lookup"><span data-stu-id="3ac20-139">address</span></span>      |[<span data-ttu-id="3ac20-140">ナビゲーション."postaladdress</span><span class="sxs-lookup"><span data-stu-id="3ac20-140">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="3ac20-141">顧客の住所を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-141">Specifies the customer's address.</span></span> <span data-ttu-id="3ac20-142">この住所は、お客様のすべてのセールスドキュメントに表示されます。</span><span class="sxs-lookup"><span data-stu-id="3ac20-142">This address will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="3ac20-143">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="3ac20-143">phoneNumber</span></span>  |<span data-ttu-id="3ac20-144">string</span><span class="sxs-lookup"><span data-stu-id="3ac20-144">string</span></span>    |<span data-ttu-id="3ac20-145">顧客の電話番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-145">Specifies the customer's telephone number.</span></span>|
|<span data-ttu-id="3ac20-146">email</span><span class="sxs-lookup"><span data-stu-id="3ac20-146">email</span></span>        |<span data-ttu-id="3ac20-147">string</span><span class="sxs-lookup"><span data-stu-id="3ac20-147">string</span></span>    |<span data-ttu-id="3ac20-148">顧客の電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-148">Specifies the customer's email address.</span></span>|
|<span data-ttu-id="3ac20-149">Web サイト</span><span class="sxs-lookup"><span data-stu-id="3ac20-149">website</span></span>      |<span data-ttu-id="3ac20-150">string</span><span class="sxs-lookup"><span data-stu-id="3ac20-150">string</span></span>    |<span data-ttu-id="3ac20-151">顧客のホームページのアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-151">Specifies the customer's home page address.</span></span>|
|<span data-ttu-id="3ac20-152">taxLiable</span><span class="sxs-lookup"><span data-stu-id="3ac20-152">taxLiable</span></span>    |<span data-ttu-id="3ac20-153">ブール値</span><span class="sxs-lookup"><span data-stu-id="3ac20-153">boolean</span></span>   |<span data-ttu-id="3ac20-154">顧客または仕入先が売上税に対して責任を負わないかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-154">Specifies if the customer or vendor is liable for sales tax.</span></span> <span data-ttu-id="3ac20-155">お客様が納税責任を持つ場合は**true**に設定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-155">Set to **true** if the customer is tax liable.</span></span>|
|<span data-ttu-id="3ac20-156">taxAreaId</span><span class="sxs-lookup"><span data-stu-id="3ac20-156">taxAreaId</span></span>    |<span data-ttu-id="3ac20-157">GUID</span><span class="sxs-lookup"><span data-stu-id="3ac20-157">GUID</span></span>      |<span data-ttu-id="3ac20-158">顧客が属する税エリアを指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-158">Specifies which tax area the customer belongs to.</span></span>|
|<span data-ttu-id="3ac20-159">taxAreaDisplayName</span><span class="sxs-lookup"><span data-stu-id="3ac20-159">taxAreaDisplayName</span></span>|<span data-ttu-id="3ac20-160">string</span><span class="sxs-lookup"><span data-stu-id="3ac20-160">string</span></span>|<span data-ttu-id="3ac20-161">顧客が属する税エリアの表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-161">Specified the display name of the tax area the customer belongs to.</span></span>|
|<span data-ttu-id="3ac20-162">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="3ac20-162">taxRegistrationNumber</span></span>|<span data-ttu-id="3ac20-163">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="3ac20-163">string, maximum size 20</span></span>|<span data-ttu-id="3ac20-164">顧客の税務登録番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-164">Specified the tax registration number of the customer.</span></span>|
|<span data-ttu-id="3ac20-165">currencyId</span><span class="sxs-lookup"><span data-stu-id="3ac20-165">currencyId</span></span>   |<span data-ttu-id="3ac20-166">GUID</span><span class="sxs-lookup"><span data-stu-id="3ac20-166">GUID</span></span>      |<span data-ttu-id="3ac20-167">顧客が使用する通貨を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-167">Specifies which currency the customer uses.</span></span>|
|<span data-ttu-id="3ac20-168">currencyCode</span><span class="sxs-lookup"><span data-stu-id="3ac20-168">currencyCode</span></span> |<span data-ttu-id="3ac20-169">数値</span><span class="sxs-lookup"><span data-stu-id="3ac20-169">numeric</span></span>   |<span data-ttu-id="3ac20-170">顧客の既定の通貨コード。</span><span class="sxs-lookup"><span data-stu-id="3ac20-170">The default currency code for the customer.</span></span>|
|<span data-ttu-id="3ac20-171">paymentTermsId</span><span class="sxs-lookup"><span data-stu-id="3ac20-171">paymentTermsId</span></span>|<span data-ttu-id="3ac20-172">GUID</span><span class="sxs-lookup"><span data-stu-id="3ac20-172">GUID</span></span>     |<span data-ttu-id="3ac20-173">顧客が使用する支払い条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-173">Specifies which payment term the customer uses.</span></span>|
|<span data-ttu-id="3ac20-174">paymentMethodId</span><span class="sxs-lookup"><span data-stu-id="3ac20-174">paymentMethodId</span></span>|<span data-ttu-id="3ac20-175">GUID</span><span class="sxs-lookup"><span data-stu-id="3ac20-175">GUID</span></span>    |<span data-ttu-id="3ac20-176">顧客が使用する支払い方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-176">Specifies which payment method the customer uses.</span></span>|
|<span data-ttu-id="3ac20-177">shipmentMethodId</span><span class="sxs-lookup"><span data-stu-id="3ac20-177">shipmentMethodId</span></span>|<span data-ttu-id="3ac20-178">GUID</span><span class="sxs-lookup"><span data-stu-id="3ac20-178">GUID</span></span>   |<span data-ttu-id="3ac20-179">顧客がどの送付方法を使用するかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-179">Specifies which shipment method the customer uses.</span></span>|
|<span data-ttu-id="3ac20-180">ブロック</span><span class="sxs-lookup"><span data-stu-id="3ac20-180">blocked</span></span>      |<span data-ttu-id="3ac20-181">string</span><span class="sxs-lookup"><span data-stu-id="3ac20-181">string</span></span>    |<span data-ttu-id="3ac20-182">顧客とのトランザクションを転記できないことを指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-182">Specifies that transactions with the customer cannot be posted.</span></span> <span data-ttu-id="3ac20-183">顧客がブロックされていない場合は、[**すべて**] に設定します。ブロックしない場合は、[空白] に設定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-183">Set to **All**, if the customer is blocked, set to blank if not blocked.</span></span>|
|<span data-ttu-id="3ac20-184">対照</span><span class="sxs-lookup"><span data-stu-id="3ac20-184">balance</span></span>      |<span data-ttu-id="3ac20-185">数値</span><span class="sxs-lookup"><span data-stu-id="3ac20-185">numeric</span></span>   |<span data-ttu-id="3ac20-186">顧客が完了した売上に対して支払うべき支払い金額を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-186">Specifies the payment amount that the customer owes for completed sales.</span></span> <span data-ttu-id="3ac20-187">この値は、顧客の残高とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="3ac20-187">This value is also known as the customer's balance.</span></span> <span data-ttu-id="3ac20-188">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3ac20-188">Read-Only.</span></span>|
|<span data-ttu-id="3ac20-189">overdueAmount</span><span class="sxs-lookup"><span data-stu-id="3ac20-189">overdueAmount</span></span>|<span data-ttu-id="3ac20-190">数値</span><span class="sxs-lookup"><span data-stu-id="3ac20-190">numeric</span></span>   |<span data-ttu-id="3ac20-191">顧客の延滞金額を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-191">Specifies the customer's overdue amount.</span></span>|
|<span data-ttu-id="3ac20-192">totalSalesExcludingTax</span><span class="sxs-lookup"><span data-stu-id="3ac20-192">totalSalesExcludingTax</span></span>|<span data-ttu-id="3ac20-193">数値</span><span class="sxs-lookup"><span data-stu-id="3ac20-193">numeric</span></span>|<span data-ttu-id="3ac20-194">顧客の税を除いた合計売上金額を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ac20-194">Specifies the total sales amount excluding tax of the customer.</span></span>|
|<span data-ttu-id="3ac20-195">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ac20-195">lastModifiedDateTime</span></span>|<span data-ttu-id="3ac20-196">datetime</span><span class="sxs-lookup"><span data-stu-id="3ac20-196">datetime</span></span>|<span data-ttu-id="3ac20-197">顧客が最後に変更された日付です。</span><span class="sxs-lookup"><span data-stu-id="3ac20-197">The last datetime the customer was modified.</span></span> <span data-ttu-id="3ac20-198">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3ac20-198">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="3ac20-199">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3ac20-199">Relationships</span></span>
<span data-ttu-id="3ac20-200">通貨 (currencyCode) は、[通貨] テーブルに存在している必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ac20-200">A Currency(currencyCode) must exist in the Currencies table.</span></span>

<span data-ttu-id="3ac20-201">支払い条件 (paymentTerms) は支払い条件テーブルに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ac20-201">A Payment Term(paymentTerms) must exist in the Payment Terms table.</span></span>

<span data-ttu-id="3ac20-202">送付方法 (shipmentMethod) は、送付方法テーブルに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ac20-202">A Shipment Method(shipmentMethod) must exist in the Shipment Method table.</span></span>

<span data-ttu-id="3ac20-203">支払い方法 ([cash]) は支払い方法テーブルに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ac20-203">A Payment Method(paymentMethod) must exist in the Payment Method table.</span></span>

<span data-ttu-id="3ac20-204">税エリア (taxArea) は、税エリアテーブルに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ac20-204">A Tax Area(taxArea) must exist in the Tax Area table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ac20-205">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3ac20-205">JSON representation</span></span>

<span data-ttu-id="3ac20-206">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3ac20-206">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "type": "string",
    "address": NAV.PostalAddress,
    "phoneNumber": "string",
    "email": "string",
    "website": "string",
    "taxLiable": "boolean",
    "taxAreaId": "GUID",
    "taxAreaDisplayName": "string",
    "taxRegistrationNumber": "string",
    "currencyCode": "string",
    "paymentTermsId": "GUID",
    "shipmentMethodId": "GUID",
    "paymentMethodId":  "GUID",
    "blocked": "string",
    "balance": "decimal",
    "overdueAmount": "numeric",
    "totalSalesExcludingTax": "numeric",
    "lastModifiedDateTime": "datetime"
}


```

