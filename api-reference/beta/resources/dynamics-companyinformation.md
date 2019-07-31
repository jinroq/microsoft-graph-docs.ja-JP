---
title: 会社情報リソースの種類
description: Dynamics 365 Business Central の会社情報。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 2e23660775ba96b3f898840b0bad2b53eff9584a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012668"
---
# <a name="companyinformation-resource-type"></a><span data-ttu-id="c7cb5-103">会社情報リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7cb5-103">companyInformation resource type</span></span>
<span data-ttu-id="c7cb5-104">Dynamics 365 Business Central の現在の会社に対して指定されている情報 (名前、住所、電子メールアドレス、web サイトのアドレスなど) を表します。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-104">Represents the information specified for the current company in Dynamics 365 Business Central, such as name, address, email address, and website address.</span></span>

## <a name="methods"></a><span data-ttu-id="c7cb5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c7cb5-105">Methods</span></span>

| <span data-ttu-id="c7cb5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c7cb5-106">Method</span></span>         | <span data-ttu-id="c7cb5-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c7cb5-107">Return Type</span></span>  |<span data-ttu-id="c7cb5-108">説明</span><span class="sxs-lookup"><span data-stu-id="c7cb5-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="c7cb5-109">会社情報の取得</span><span class="sxs-lookup"><span data-stu-id="c7cb5-109">Get companyInformation</span></span>](../api/dynamics-companyinformation-get.md)|<span data-ttu-id="c7cb5-110">会社情報</span><span class="sxs-lookup"><span data-stu-id="c7cb5-110">companyInformation</span></span>|<span data-ttu-id="c7cb5-111">会社の情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-111">Gets a company information.</span></span>|
|[<span data-ttu-id="c7cb5-112">パッチ会社の情報</span><span class="sxs-lookup"><span data-stu-id="c7cb5-112">Patch companyInformation</span></span>](../api/dynamics-companyinformation-update.md)|<span data-ttu-id="c7cb5-113">会社情報</span><span class="sxs-lookup"><span data-stu-id="c7cb5-113">companyInformation</span></span>|<span data-ttu-id="c7cb5-114">会社情報を更新します。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-114">Updates a company information.</span></span>|


## <a name="properties"></a><span data-ttu-id="c7cb5-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7cb5-115">Properties</span></span>
| <span data-ttu-id="c7cb5-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7cb5-116">Property</span></span>     | <span data-ttu-id="c7cb5-117">型</span><span class="sxs-lookup"><span data-stu-id="c7cb5-117">Type</span></span>      |<span data-ttu-id="c7cb5-118">説明</span><span class="sxs-lookup"><span data-stu-id="c7cb5-118">Description</span></span>                           |
|:-------------|:--------|:-------------------------------------|
|<span data-ttu-id="c7cb5-119">id</span><span class="sxs-lookup"><span data-stu-id="c7cb5-119">id</span></span>            |<span data-ttu-id="c7cb5-120">GUID</span><span class="sxs-lookup"><span data-stu-id="c7cb5-120">GUID</span></span>|<span data-ttu-id="c7cb5-121">会社の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-121">The unique ID of the company.</span></span> <span data-ttu-id="c7cb5-122">編集できません。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-122">Non-editable.</span></span>|
|<span data-ttu-id="c7cb5-123">displayName</span><span class="sxs-lookup"><span data-stu-id="c7cb5-123">displayName</span></span>   |<span data-ttu-id="c7cb5-124">string</span><span class="sxs-lookup"><span data-stu-id="c7cb5-124">string</span></span>   |<span data-ttu-id="c7cb5-125">会社の表示名。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-125">The company's display name.</span></span>           |
|<span data-ttu-id="c7cb5-126">address</span><span class="sxs-lookup"><span data-stu-id="c7cb5-126">address</span></span>       |[<span data-ttu-id="c7cb5-127">ナビゲーション."Postaladdress</span><span class="sxs-lookup"><span data-stu-id="c7cb5-127">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="c7cb5-128">会社の住所。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-128">The company's address.</span></span> <span data-ttu-id="c7cb5-129">詳細については、「複合型」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-129">View the complex type for additional detail.</span></span>|
|<span data-ttu-id="c7cb5-130">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="c7cb5-130">phoneNumber</span></span>   |<span data-ttu-id="c7cb5-131">string</span><span class="sxs-lookup"><span data-stu-id="c7cb5-131">string</span></span>   |<span data-ttu-id="c7cb5-132">会社の電話番号。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-132">The company's telephone number.</span></span>       |
|<span data-ttu-id="c7cb5-133">faxNumber</span><span class="sxs-lookup"><span data-stu-id="c7cb5-133">faxNumber</span></span>     |<span data-ttu-id="c7cb5-134">string</span><span class="sxs-lookup"><span data-stu-id="c7cb5-134">string</span></span>   |<span data-ttu-id="c7cb5-135">会社の fax 番号。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-135">The company's fax number.</span></span>             |
|<span data-ttu-id="c7cb5-136">email</span><span class="sxs-lookup"><span data-stu-id="c7cb5-136">email</span></span>         |<span data-ttu-id="c7cb5-137">string</span><span class="sxs-lookup"><span data-stu-id="c7cb5-137">string</span></span>   |<span data-ttu-id="c7cb5-138">会社の電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-138">The company's email address.</span></span>          |
|<span data-ttu-id="c7cb5-139">Web サイト</span><span class="sxs-lookup"><span data-stu-id="c7cb5-139">website</span></span>       |<span data-ttu-id="c7cb5-140">string</span><span class="sxs-lookup"><span data-stu-id="c7cb5-140">string</span></span>   |<span data-ttu-id="c7cb5-141">会社の web サイトアドレス。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-141">The company's website address.</span></span>        |
|<span data-ttu-id="c7cb5-142">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="c7cb5-142">taxRegistrationNumber</span></span>|<span data-ttu-id="c7cb5-143">string</span><span class="sxs-lookup"><span data-stu-id="c7cb5-143">string</span></span>|<span data-ttu-id="c7cb5-144">会社の税務登録番号。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-144">The company's tax registration number.</span></span>|
|<span data-ttu-id="c7cb5-145">currencyCode</span><span class="sxs-lookup"><span data-stu-id="c7cb5-145">currencyCode</span></span>  |<span data-ttu-id="c7cb5-146">string</span><span class="sxs-lookup"><span data-stu-id="c7cb5-146">string</span></span>   |<span data-ttu-id="c7cb5-147">会社が事業を行う通貨。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-147">The currency the company does business in.</span></span> <span data-ttu-id="c7cb5-148">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-148">Read-Only.</span></span>|
|<span data-ttu-id="c7cb5-149">currentFiscalYearStartDate</span><span class="sxs-lookup"><span data-stu-id="c7cb5-149">currentFiscalYearStartDate</span></span>|<span data-ttu-id="c7cb5-150">date</span><span class="sxs-lookup"><span data-stu-id="c7cb5-150">date</span></span>|<span data-ttu-id="c7cb5-151">会社の現在の会計年度の開始日。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-151">The company's current fiscal year start date.</span></span> <span data-ttu-id="c7cb5-152">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-152">Read-Only.</span></span>|
|<span data-ttu-id="c7cb5-153">おける</span><span class="sxs-lookup"><span data-stu-id="c7cb5-153">industry</span></span>      |<span data-ttu-id="c7cb5-154">string</span><span class="sxs-lookup"><span data-stu-id="c7cb5-154">string</span></span>   |<span data-ttu-id="c7cb5-155">会社が属している業界。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-155">The industry the company is part of.</span></span>  |
|<span data-ttu-id="c7cb5-156">表</span><span class="sxs-lookup"><span data-stu-id="c7cb5-156">picture</span></span>       |<span data-ttu-id="c7cb5-157">stream</span><span class="sxs-lookup"><span data-stu-id="c7cb5-157">stream</span></span>   |<span data-ttu-id="c7cb5-158">会社のロゴ。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-158">The company logo.</span></span> <span data-ttu-id="c7cb5-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-159">Read-Only.</span></span>          |
|<span data-ttu-id="c7cb5-160">businessProfileId</span><span class="sxs-lookup"><span data-stu-id="c7cb5-160">businessProfileId</span></span>|<span data-ttu-id="c7cb5-161">string</span><span class="sxs-lookup"><span data-stu-id="c7cb5-161">string</span></span>|<span data-ttu-id="c7cb5-162">財務会社にリンクされているビジネスプロファイル ID。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-162">The business profile ID linked to the Financials company.</span></span> <span data-ttu-id="c7cb5-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-163">Read-Only.</span></span>|
|<span data-ttu-id="c7cb5-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7cb5-164">lastModifiedDateTime</span></span>|<span data-ttu-id="c7cb5-165">datetime</span><span class="sxs-lookup"><span data-stu-id="c7cb5-165">datetime</span></span>|<span data-ttu-id="c7cb5-166">会社が変更された最後の日付です。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-166">The last datetime the company was modified.</span></span> <span data-ttu-id="c7cb5-167">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-167">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="c7cb5-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c7cb5-168">Relationships</span></span>
<span data-ttu-id="c7cb5-169">なし</span><span class="sxs-lookup"><span data-stu-id="c7cb5-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7cb5-170">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7cb5-170">JSON representation</span></span>

<span data-ttu-id="c7cb5-171">会社情報の JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c7cb5-171">Here is a JSON representation of the companyInformation</span></span>
```json
{
  "id": "GUID",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "faxNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyCode": "string",
  "currentFiscalYearStartDate": "date",
  "industry": "string",
  "picture": "stream",
  "businessProfileId": "string",
  "lastModifiedDateTime": "datetime"
}

```

