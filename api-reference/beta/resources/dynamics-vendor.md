---
title: ベンダーリソースの種類
description: Dynamics 365 Business Central のベンダーオブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 7c0609d96f6d97503faf5c5251d3641979a4f6e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972853"
---
# <a name="vendors-resource-type"></a><span data-ttu-id="8892a-103">ベンダーリソースの種類</span><span class="sxs-lookup"><span data-stu-id="8892a-103">vendors resource type</span></span>
<span data-ttu-id="8892a-104">Dynamics 365 Business Central のベンダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8892a-104">Represents a vendor in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="8892a-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="8892a-105">Methods</span></span>

| <span data-ttu-id="8892a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8892a-106">Method</span></span>       | <span data-ttu-id="8892a-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8892a-107">Return Type</span></span>  |<span data-ttu-id="8892a-108">説明</span><span class="sxs-lookup"><span data-stu-id="8892a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8892a-109">ベンダーを取得する</span><span class="sxs-lookup"><span data-stu-id="8892a-109">Get vendors</span></span>](../api/dynamics-vendor-get.md)|<span data-ttu-id="8892a-110">主要</span><span class="sxs-lookup"><span data-stu-id="8892a-110">vendors</span></span>|<span data-ttu-id="8892a-111">ベンダーオブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="8892a-111">Gets a vendor object.</span></span>|
|[<span data-ttu-id="8892a-112">ベンダーを投稿する</span><span class="sxs-lookup"><span data-stu-id="8892a-112">Post vendors</span></span>](../api/dynamics-create-vendor.md)|<span data-ttu-id="8892a-113">主要</span><span class="sxs-lookup"><span data-stu-id="8892a-113">vendors</span></span>|<span data-ttu-id="8892a-114">ベンダーオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8892a-114">Creates a vendor object.</span></span>|
|[<span data-ttu-id="8892a-115">パッチベンダー</span><span class="sxs-lookup"><span data-stu-id="8892a-115">Patch vendors</span></span>](../api/dynamics-vendor-update.md)|<span data-ttu-id="8892a-116">主要</span><span class="sxs-lookup"><span data-stu-id="8892a-116">vendors</span></span>|<span data-ttu-id="8892a-117">ベンダーオブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="8892a-117">Updates a vendor object.</span></span>|
|[<span data-ttu-id="8892a-118">仕入先を削除する</span><span class="sxs-lookup"><span data-stu-id="8892a-118">Delete vendor</span></span>](../api/dynamics-vendor-delete.md)|<span data-ttu-id="8892a-119">none</span><span class="sxs-lookup"><span data-stu-id="8892a-119">none</span></span>|<span data-ttu-id="8892a-120">ベンダーオブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="8892a-120">Deletes a vendor object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8892a-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8892a-121">Properties</span></span>
| <span data-ttu-id="8892a-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8892a-122">Property</span></span>     | <span data-ttu-id="8892a-123">型</span><span class="sxs-lookup"><span data-stu-id="8892a-123">Type</span></span>   |<span data-ttu-id="8892a-124">説明</span><span class="sxs-lookup"><span data-stu-id="8892a-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8892a-125">id</span><span class="sxs-lookup"><span data-stu-id="8892a-125">id</span></span>|<span data-ttu-id="8892a-126">GUID</span><span class="sxs-lookup"><span data-stu-id="8892a-126">GUID</span></span>|<span data-ttu-id="8892a-127">ベンダーの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="8892a-127">The unique ID of the vendor.</span></span> <span data-ttu-id="8892a-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="8892a-128">Non-editable.</span></span>|
|<span data-ttu-id="8892a-129">番号</span><span class="sxs-lookup"><span data-stu-id="8892a-129">number</span></span>|<span data-ttu-id="8892a-130">string</span><span class="sxs-lookup"><span data-stu-id="8892a-130">string</span></span>|<span data-ttu-id="8892a-131">仕入先番号。</span><span class="sxs-lookup"><span data-stu-id="8892a-131">The vendor number.</span></span>|
|<span data-ttu-id="8892a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8892a-132">displayName</span></span>|<span data-ttu-id="8892a-133">string</span><span class="sxs-lookup"><span data-stu-id="8892a-133">string</span></span>|<span data-ttu-id="8892a-134">仕入先の表示名。</span><span class="sxs-lookup"><span data-stu-id="8892a-134">The vendor's display name.</span></span>|
|<span data-ttu-id="8892a-135">address</span><span class="sxs-lookup"><span data-stu-id="8892a-135">address</span></span>|[<span data-ttu-id="8892a-136">ナビゲーション."Postaladdress</span><span class="sxs-lookup"><span data-stu-id="8892a-136">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="8892a-137">仕入先の住所。</span><span class="sxs-lookup"><span data-stu-id="8892a-137">The vendor's address.</span></span>|
|<span data-ttu-id="8892a-138">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="8892a-138">phoneNumber</span></span>|<span data-ttu-id="8892a-139">string</span><span class="sxs-lookup"><span data-stu-id="8892a-139">string</span></span>|<span data-ttu-id="8892a-140">仕入先の電話番号。</span><span class="sxs-lookup"><span data-stu-id="8892a-140">The vendor's telephone number.</span></span>|
|<span data-ttu-id="8892a-141">email</span><span class="sxs-lookup"><span data-stu-id="8892a-141">email</span></span>|<span data-ttu-id="8892a-142">string</span><span class="sxs-lookup"><span data-stu-id="8892a-142">string</span></span>|<span data-ttu-id="8892a-143">仕入先の電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="8892a-143">The vendor's email address.</span></span>|
|<span data-ttu-id="8892a-144">Web サイト</span><span class="sxs-lookup"><span data-stu-id="8892a-144">website</span></span>|<span data-ttu-id="8892a-145">string</span><span class="sxs-lookup"><span data-stu-id="8892a-145">string</span></span>|<span data-ttu-id="8892a-146">ベンダーの web サイトアドレス。</span><span class="sxs-lookup"><span data-stu-id="8892a-146">The vendor's website address.</span></span>|
|<span data-ttu-id="8892a-147">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="8892a-147">taxRegistrationNumber</span></span>|<span data-ttu-id="8892a-148">string</span><span class="sxs-lookup"><span data-stu-id="8892a-148">string</span></span>|<span data-ttu-id="8892a-149">仕入先の税登録番号。</span><span class="sxs-lookup"><span data-stu-id="8892a-149">The vendor's tax registration number.</span></span>|
|<span data-ttu-id="8892a-150">currencyId</span><span class="sxs-lookup"><span data-stu-id="8892a-150">currencyId</span></span>|<span data-ttu-id="8892a-151">GUID</span><span class="sxs-lookup"><span data-stu-id="8892a-151">GUID</span></span>|<span data-ttu-id="8892a-152">仕入先の既定通貨コード ID。</span><span class="sxs-lookup"><span data-stu-id="8892a-152">The default currency code ID for the vendor.</span></span>|
|<span data-ttu-id="8892a-153">currencyCode</span><span class="sxs-lookup"><span data-stu-id="8892a-153">currencyCode</span></span>|<span data-ttu-id="8892a-154">string</span><span class="sxs-lookup"><span data-stu-id="8892a-154">string</span></span>|<span data-ttu-id="8892a-155">仕入先の既定の通貨コード。</span><span class="sxs-lookup"><span data-stu-id="8892a-155">The default currency code for the vendor.</span></span>|
|<span data-ttu-id="8892a-156">irs1099Code</span><span class="sxs-lookup"><span data-stu-id="8892a-156">irs1099Code</span></span>|<span data-ttu-id="8892a-157">string</span><span class="sxs-lookup"><span data-stu-id="8892a-157">string</span></span>|<span data-ttu-id="8892a-158">ベンダーの1099コードを指定します。</span><span class="sxs-lookup"><span data-stu-id="8892a-158">Specifies a 1099 code for the vendor.</span></span> <span data-ttu-id="8892a-159">US のみ</span><span class="sxs-lookup"><span data-stu-id="8892a-159">US only.</span></span>|
|<span data-ttu-id="8892a-160">paymentTermsId</span><span class="sxs-lookup"><span data-stu-id="8892a-160">paymentTermsId</span></span>|<span data-ttu-id="8892a-161">GUID</span><span class="sxs-lookup"><span data-stu-id="8892a-161">GUID</span></span>|<span data-ttu-id="8892a-162">仕入先の既定の支払条件 ID。</span><span class="sxs-lookup"><span data-stu-id="8892a-162">The default payment terms ID for the vendor.</span></span>|
|<span data-ttu-id="8892a-163">paymentMethodId</span><span class="sxs-lookup"><span data-stu-id="8892a-163">paymentMethodId</span></span>|<span data-ttu-id="8892a-164">GUID</span><span class="sxs-lookup"><span data-stu-id="8892a-164">GUID</span></span>|<span data-ttu-id="8892a-165">仕入先の既定の支払方法 ID。</span><span class="sxs-lookup"><span data-stu-id="8892a-165">The default payment method ID for the vendor.</span></span>|
|<span data-ttu-id="8892a-166">taxLiable</span><span class="sxs-lookup"><span data-stu-id="8892a-166">taxLiable</span></span>|<span data-ttu-id="8892a-167">ブール値</span><span class="sxs-lookup"><span data-stu-id="8892a-167">boolean</span></span>|<span data-ttu-id="8892a-168">仕入先が税金に対して責任を負わないかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8892a-168">Specifies if the vendor is liable for tax.</span></span>|
|<span data-ttu-id="8892a-169">ブロック</span><span class="sxs-lookup"><span data-stu-id="8892a-169">blocked</span></span>|<span data-ttu-id="8892a-170">string</span><span class="sxs-lookup"><span data-stu-id="8892a-170">string</span></span>|<span data-ttu-id="8892a-171">転記できない仕入先のトランザクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="8892a-171">Specifies which transactions with the vendor that cannot be posted.</span></span> <span data-ttu-id="8892a-172">指定できる値は空白、支払いまたはすべてです</span><span class="sxs-lookup"><span data-stu-id="8892a-172">Accepted values are blank, Payment or All</span></span>|
|<span data-ttu-id="8892a-173">対照</span><span class="sxs-lookup"><span data-stu-id="8892a-173">balance</span></span>|<span data-ttu-id="8892a-174">decimal</span><span class="sxs-lookup"><span data-stu-id="8892a-174">decimal</span></span>|<span data-ttu-id="8892a-175">仕入先の残高。</span><span class="sxs-lookup"><span data-stu-id="8892a-175">The vendor's balance.</span></span> <span data-ttu-id="8892a-176">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8892a-176">Read-Only.</span></span>|
|<span data-ttu-id="8892a-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8892a-177">lastModifiedDateTime</span></span>|<span data-ttu-id="8892a-178">datetime</span><span class="sxs-lookup"><span data-stu-id="8892a-178">datetime</span></span>|<span data-ttu-id="8892a-179">ベンダーが最後に変更された datetime。</span><span class="sxs-lookup"><span data-stu-id="8892a-179">The last datetime the vendor was modified.</span></span> <span data-ttu-id="8892a-180">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="8892a-180">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="8892a-181">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8892a-181">Relationships</span></span>
<span data-ttu-id="8892a-182">なし</span><span class="sxs-lookup"><span data-stu-id="8892a-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8892a-183">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8892a-183">JSON representation</span></span>

<span data-ttu-id="8892a-184">以下は、ベンダーの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8892a-184">Here is a JSON representation of the vendor.</span></span>

```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyId": "GUID",
  "currencyCode": "string",
  "irs1099Code": "string",
  "paymentTermsId": "GUID",
  "paymentMethodId": "GUID",
  "taxLiable": "boolean",
  "blocked": "string",
  "balance": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

