---
title: customers リソースの種類
description: Dynamics 365 Business Central の顧客を表します。
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 2a3ad7bade33af9456e65e3c19b988b9d2f679b2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973640"
---
# <a name="customers-resource-type"></a><span data-ttu-id="c8b83-103">customers リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8b83-103">customers resource type</span></span>
<span data-ttu-id="c8b83-104">Dynamics 365 Business Central の顧客を表します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-104">Represents a customer in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="c8b83-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c8b83-105">Methods</span></span>

| <span data-ttu-id="c8b83-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c8b83-106">Method</span></span>                                              |<span data-ttu-id="c8b83-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c8b83-107">Return Type</span></span>| <span data-ttu-id="c8b83-108">説明</span><span class="sxs-lookup"><span data-stu-id="c8b83-108">Description</span></span>      |
|:----------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="c8b83-109">顧客を取得する</span><span class="sxs-lookup"><span data-stu-id="c8b83-109">Get customers</span></span>](../api/dynamics-customer-get.md)      |<span data-ttu-id="c8b83-110">ユーザー</span><span class="sxs-lookup"><span data-stu-id="c8b83-110">customers</span></span>   |<span data-ttu-id="c8b83-111">顧客を取得します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-111">Gets a customer.</span></span>   |
|[<span data-ttu-id="c8b83-112">顧客を作成する</span><span class="sxs-lookup"><span data-stu-id="c8b83-112">Create customers</span></span>](../api/dynamics-create-customer.md)|<span data-ttu-id="c8b83-113">ユーザー</span><span class="sxs-lookup"><span data-stu-id="c8b83-113">customers</span></span>   |<span data-ttu-id="c8b83-114">顧客を作成します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-114">Creates a customer.</span></span>|
|[<span data-ttu-id="c8b83-115">顧客を更新する</span><span class="sxs-lookup"><span data-stu-id="c8b83-115">Update customers</span></span>](../api/dynamics-customer-update.md)|<span data-ttu-id="c8b83-116">ユーザー</span><span class="sxs-lookup"><span data-stu-id="c8b83-116">customers</span></span>   |<span data-ttu-id="c8b83-117">顧客を更新します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-117">Updates a customer.</span></span>|
|[<span data-ttu-id="c8b83-118">顧客を削除する</span><span class="sxs-lookup"><span data-stu-id="c8b83-118">Delete customers</span></span>](../api/dynamics-customer-delete.md)|<span data-ttu-id="c8b83-119">none</span><span class="sxs-lookup"><span data-stu-id="c8b83-119">none</span></span>        |<span data-ttu-id="c8b83-120">顧客を削除します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-120">Deletes a customer.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8b83-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8b83-121">Properties</span></span>
| <span data-ttu-id="c8b83-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8b83-122">Property</span></span>    | <span data-ttu-id="c8b83-123">型</span><span class="sxs-lookup"><span data-stu-id="c8b83-123">Type</span></span>     |<span data-ttu-id="c8b83-124">説明</span><span class="sxs-lookup"><span data-stu-id="c8b83-124">Description</span></span>|
|:------------|:---------|:----------|
|<span data-ttu-id="c8b83-125">id</span><span class="sxs-lookup"><span data-stu-id="c8b83-125">id</span></span>           |<span data-ttu-id="c8b83-126">GUID</span><span class="sxs-lookup"><span data-stu-id="c8b83-126">GUID</span></span>      |<span data-ttu-id="c8b83-127">アイテムの一意の ID です。</span><span class="sxs-lookup"><span data-stu-id="c8b83-127">The unique ID of the item.</span></span> <span data-ttu-id="c8b83-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="c8b83-128">Non-editable.</span></span>|
|<span data-ttu-id="c8b83-129">番号</span><span class="sxs-lookup"><span data-stu-id="c8b83-129">number</span></span>       |<span data-ttu-id="c8b83-130">string</span><span class="sxs-lookup"><span data-stu-id="c8b83-130">string</span></span>    |<span data-ttu-id="c8b83-131">顧客番号。</span><span class="sxs-lookup"><span data-stu-id="c8b83-131">The customer number.</span></span>|
|<span data-ttu-id="c8b83-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c8b83-132">displayName</span></span>  |<span data-ttu-id="c8b83-133">string</span><span class="sxs-lookup"><span data-stu-id="c8b83-133">string</span></span>    |<span data-ttu-id="c8b83-134">顧客の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-134">Specifies the customer's name.</span></span> <span data-ttu-id="c8b83-135">この名前は、顧客のすべての販売ドキュメントに表示されます。</span><span class="sxs-lookup"><span data-stu-id="c8b83-135">This name will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="c8b83-136">type</span><span class="sxs-lookup"><span data-stu-id="c8b83-136">type</span></span>         |<span data-ttu-id="c8b83-137">string</span><span class="sxs-lookup"><span data-stu-id="c8b83-137">string</span></span>    |<span data-ttu-id="c8b83-138">顧客の種類として、"Company" または "Person" を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-138">Specifies the type of customer, can be "Company" or "Person".</span></span>|
|<span data-ttu-id="c8b83-139">address</span><span class="sxs-lookup"><span data-stu-id="c8b83-139">address</span></span>      |[<span data-ttu-id="c8b83-140">ナビゲーション."Postaladdress</span><span class="sxs-lookup"><span data-stu-id="c8b83-140">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="c8b83-141">顧客の住所を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-141">Specifies the customer's address.</span></span> <span data-ttu-id="c8b83-142">この住所は、お客様のすべてのセールスドキュメントに表示されます。</span><span class="sxs-lookup"><span data-stu-id="c8b83-142">This address will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="c8b83-143">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="c8b83-143">phoneNumber</span></span>  |<span data-ttu-id="c8b83-144">string</span><span class="sxs-lookup"><span data-stu-id="c8b83-144">string</span></span>    |<span data-ttu-id="c8b83-145">顧客の電話番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-145">Specifies the customer's telephone number.</span></span>|
|<span data-ttu-id="c8b83-146">email</span><span class="sxs-lookup"><span data-stu-id="c8b83-146">email</span></span>        |<span data-ttu-id="c8b83-147">string</span><span class="sxs-lookup"><span data-stu-id="c8b83-147">string</span></span>    |<span data-ttu-id="c8b83-148">顧客の電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-148">Specifies the customer's email address.</span></span>|
|<span data-ttu-id="c8b83-149">Web サイト</span><span class="sxs-lookup"><span data-stu-id="c8b83-149">website</span></span>      |<span data-ttu-id="c8b83-150">string</span><span class="sxs-lookup"><span data-stu-id="c8b83-150">string</span></span>    |<span data-ttu-id="c8b83-151">顧客のホームページのアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-151">Specifies the customer's home page address.</span></span>|
|<span data-ttu-id="c8b83-152">taxLiable</span><span class="sxs-lookup"><span data-stu-id="c8b83-152">taxLiable</span></span>    |<span data-ttu-id="c8b83-153">ブール値</span><span class="sxs-lookup"><span data-stu-id="c8b83-153">boolean</span></span>   |<span data-ttu-id="c8b83-154">顧客または仕入先が売上税に対して責任を負わないかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-154">Specifies if the customer or vendor is liable for sales tax.</span></span> <span data-ttu-id="c8b83-155">お客様が納税責任を持つ場合は**true**に設定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-155">Set to **true** if the customer is tax liable.</span></span>|
|<span data-ttu-id="c8b83-156">taxAreaId</span><span class="sxs-lookup"><span data-stu-id="c8b83-156">taxAreaId</span></span>    |<span data-ttu-id="c8b83-157">GUID</span><span class="sxs-lookup"><span data-stu-id="c8b83-157">GUID</span></span>      |<span data-ttu-id="c8b83-158">顧客が属する税エリアを指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-158">Specifies which tax area the customer belongs to.</span></span>|
|<span data-ttu-id="c8b83-159">taxAreaDisplayName</span><span class="sxs-lookup"><span data-stu-id="c8b83-159">taxAreaDisplayName</span></span>|<span data-ttu-id="c8b83-160">string</span><span class="sxs-lookup"><span data-stu-id="c8b83-160">string</span></span>|<span data-ttu-id="c8b83-161">顧客が属する税エリアの表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-161">Specified the display name of the tax area the customer belongs to.</span></span>|
|<span data-ttu-id="c8b83-162">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="c8b83-162">taxRegistrationNumber</span></span>|<span data-ttu-id="c8b83-163">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="c8b83-163">string, maximum size 20</span></span>|<span data-ttu-id="c8b83-164">顧客の税務登録番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-164">Specified the tax registration number of the customer.</span></span>|
|<span data-ttu-id="c8b83-165">currencyId</span><span class="sxs-lookup"><span data-stu-id="c8b83-165">currencyId</span></span>   |<span data-ttu-id="c8b83-166">GUID</span><span class="sxs-lookup"><span data-stu-id="c8b83-166">GUID</span></span>      |<span data-ttu-id="c8b83-167">顧客が使用する通貨を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-167">Specifies which currency the customer uses.</span></span>|
|<span data-ttu-id="c8b83-168">currencyCode</span><span class="sxs-lookup"><span data-stu-id="c8b83-168">currencyCode</span></span> |<span data-ttu-id="c8b83-169">数値</span><span class="sxs-lookup"><span data-stu-id="c8b83-169">numeric</span></span>   |<span data-ttu-id="c8b83-170">顧客の既定の通貨コード。</span><span class="sxs-lookup"><span data-stu-id="c8b83-170">The default currency code for the customer.</span></span>|
|<span data-ttu-id="c8b83-171">paymentTermsId</span><span class="sxs-lookup"><span data-stu-id="c8b83-171">paymentTermsId</span></span>|<span data-ttu-id="c8b83-172">GUID</span><span class="sxs-lookup"><span data-stu-id="c8b83-172">GUID</span></span>     |<span data-ttu-id="c8b83-173">顧客が使用する支払い条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-173">Specifies which payment term the customer uses.</span></span>|
|<span data-ttu-id="c8b83-174">paymentMethodId</span><span class="sxs-lookup"><span data-stu-id="c8b83-174">paymentMethodId</span></span>|<span data-ttu-id="c8b83-175">GUID</span><span class="sxs-lookup"><span data-stu-id="c8b83-175">GUID</span></span>    |<span data-ttu-id="c8b83-176">顧客が使用する支払い方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-176">Specifies which payment method the customer uses.</span></span>|
|<span data-ttu-id="c8b83-177">shipmentMethodId</span><span class="sxs-lookup"><span data-stu-id="c8b83-177">shipmentMethodId</span></span>|<span data-ttu-id="c8b83-178">GUID</span><span class="sxs-lookup"><span data-stu-id="c8b83-178">GUID</span></span>   |<span data-ttu-id="c8b83-179">顧客がどの送付方法を使用するかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-179">Specifies which shipment method the customer uses.</span></span>|
|<span data-ttu-id="c8b83-180">ブロック</span><span class="sxs-lookup"><span data-stu-id="c8b83-180">blocked</span></span>      |<span data-ttu-id="c8b83-181">string</span><span class="sxs-lookup"><span data-stu-id="c8b83-181">string</span></span>    |<span data-ttu-id="c8b83-182">顧客とのトランザクションを転記できないことを指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-182">Specifies that transactions with the customer cannot be posted.</span></span> <span data-ttu-id="c8b83-183">顧客がブロックされていない場合は、[**すべて**] に設定します。ブロックしない場合は、[空白] に設定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-183">Set to **All**, if the customer is blocked, set to blank if not blocked.</span></span>|
|<span data-ttu-id="c8b83-184">対照</span><span class="sxs-lookup"><span data-stu-id="c8b83-184">balance</span></span>      |<span data-ttu-id="c8b83-185">数値</span><span class="sxs-lookup"><span data-stu-id="c8b83-185">numeric</span></span>   |<span data-ttu-id="c8b83-186">顧客が完了した売上に対して支払うべき支払い金額を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-186">Specifies the payment amount that the customer owes for completed sales.</span></span> <span data-ttu-id="c8b83-187">この値は、顧客の残高とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="c8b83-187">This value is also known as the customer's balance.</span></span> <span data-ttu-id="c8b83-188">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c8b83-188">Read-Only.</span></span>|
|<span data-ttu-id="c8b83-189">overdueAmount</span><span class="sxs-lookup"><span data-stu-id="c8b83-189">overdueAmount</span></span>|<span data-ttu-id="c8b83-190">数値</span><span class="sxs-lookup"><span data-stu-id="c8b83-190">numeric</span></span>   |<span data-ttu-id="c8b83-191">顧客の延滞金額を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-191">Specifies the customer's overdue amount.</span></span>|
|<span data-ttu-id="c8b83-192">totalSalesExcludingTax</span><span class="sxs-lookup"><span data-stu-id="c8b83-192">totalSalesExcludingTax</span></span>|<span data-ttu-id="c8b83-193">数値</span><span class="sxs-lookup"><span data-stu-id="c8b83-193">numeric</span></span>|<span data-ttu-id="c8b83-194">顧客の税を除いた合計売上金額を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8b83-194">Specifies the total sales amount excluding tax of the customer.</span></span>|
|<span data-ttu-id="c8b83-195">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8b83-195">lastModifiedDateTime</span></span>|<span data-ttu-id="c8b83-196">datetime</span><span class="sxs-lookup"><span data-stu-id="c8b83-196">datetime</span></span>|<span data-ttu-id="c8b83-197">顧客が最後に変更された日付です。</span><span class="sxs-lookup"><span data-stu-id="c8b83-197">The last datetime the customer was modified.</span></span> <span data-ttu-id="c8b83-198">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="c8b83-198">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="c8b83-199">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c8b83-199">Relationships</span></span>
<span data-ttu-id="c8b83-200">通貨 (currencyCode) は、[通貨] テーブルに存在している必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8b83-200">A Currency(currencyCode) must exist in the Currencies table.</span></span>

<span data-ttu-id="c8b83-201">支払い条件 (paymentTerms) は支払い条件テーブルに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8b83-201">A Payment Term(paymentTerms) must exist in the Payment Terms table.</span></span>

<span data-ttu-id="c8b83-202">送付方法 (shipmentMethod) は、送付方法テーブルに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8b83-202">A Shipment Method(shipmentMethod) must exist in the Shipment Method table.</span></span>

<span data-ttu-id="c8b83-203">支払い方法 ([Cash]) は支払い方法テーブルに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8b83-203">A Payment Method(paymentMethod) must exist in the Payment Method table.</span></span>

<span data-ttu-id="c8b83-204">税エリア (taxArea) は、税エリアテーブルに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8b83-204">A Tax Area(taxArea) must exist in the Tax Area table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8b83-205">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8b83-205">JSON representation</span></span>

<span data-ttu-id="c8b83-206">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c8b83-206">Here is a JSON representation of the resource.</span></span>


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

