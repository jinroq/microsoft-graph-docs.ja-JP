---
author: simonhult
description: columnDefinition リソースの PersonOrGroupColumn は、列の値がディレクトリから選択した個人またはグループを表すことを示しています。
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 24daf2ffd48e7647c898031aee634e8a84e05ee0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966154"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="0c15d-103">PersonOrGroupColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c15d-103">PersonOrGroupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c15d-104">[columnDefinition](columndefinition.md) リソースの **PersonOrGroupColumn** は、列の値がディレクトリから選択した個人またはグループを表すことを示しています。</span><span class="sxs-lookup"><span data-stu-id="0c15d-104">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c15d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c15d-105">JSON representation</span></span>

<span data-ttu-id="0c15d-106">以下は、**personOrGroupColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0c15d-106">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="0c15d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c15d-107">Properties</span></span>

| <span data-ttu-id="0c15d-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="0c15d-108">Property name</span></span>              | <span data-ttu-id="0c15d-109">種類</span><span class="sxs-lookup"><span data-stu-id="0c15d-109">Type</span></span>    | <span data-ttu-id="0c15d-110">説明</span><span class="sxs-lookup"><span data-stu-id="0c15d-110">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="0c15d-111">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="0c15d-111">**allowMultipleSelection**</span></span> | <span data-ttu-id="0c15d-112">boolean</span><span class="sxs-lookup"><span data-stu-id="0c15d-112">boolean</span></span> | <span data-ttu-id="0c15d-113">ソースから複数の値を選択できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0c15d-113">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="0c15d-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="0c15d-114">**displayAs**</span></span>              | <span data-ttu-id="0c15d-115">string</span><span class="sxs-lookup"><span data-stu-id="0c15d-115">string</span></span>  | <span data-ttu-id="0c15d-116">選択された個人またはグループについての情報を表示する方法。</span><span class="sxs-lookup"><span data-stu-id="0c15d-116">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="0c15d-117">以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c15d-117">See below.</span></span>
| <span data-ttu-id="0c15d-118">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="0c15d-118">**chooseFromType**</span></span>         | <span data-ttu-id="0c15d-119">string</span><span class="sxs-lookup"><span data-stu-id="0c15d-119">string</span></span>  | <span data-ttu-id="0c15d-120">個人のみ選択、または個人とグループの選択が可能かどうか。</span><span class="sxs-lookup"><span data-stu-id="0c15d-120">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="0c15d-121">`peopleAndGroups` または `peopleOnly` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="0c15d-121">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="0c15d-122">DisplayAs 値</span><span class="sxs-lookup"><span data-stu-id="0c15d-122">DisplayAs values</span></span>

| <span data-ttu-id="0c15d-123">DisplayAs 値</span><span class="sxs-lookup"><span data-stu-id="0c15d-123">DisplayAs value</span></span>               | <span data-ttu-id="0c15d-124">説明</span><span class="sxs-lookup"><span data-stu-id="0c15d-124">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="0c15d-125">**account**</span><span class="sxs-lookup"><span data-stu-id="0c15d-125">**account**</span></span>                   | <span data-ttu-id="0c15d-126">個人またはグループの、未加工の SharePoint エンコードの要求文字列 (たとえば </span><span class="sxs-lookup"><span data-stu-id="0c15d-126">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="0c15d-127">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="0c15d-127">i:0#.f</span></span>|<span data-ttu-id="0c15d-128">membership</span><span class="sxs-lookup"><span data-stu-id="0c15d-128">membership</span></span>|<span data-ttu-id="0c15d-129">jane@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="0c15d-129">jane@contoso.com).</span></span>
| <span data-ttu-id="0c15d-130">**department**</span><span class="sxs-lookup"><span data-stu-id="0c15d-130">**department**</span></span>                | <span data-ttu-id="0c15d-131">個人またはグループの部門。</span><span class="sxs-lookup"><span data-stu-id="0c15d-131">The person or group's department.</span></span>
| <span data-ttu-id="0c15d-132">**firstName**</span><span class="sxs-lookup"><span data-stu-id="0c15d-132">**firstName**</span></span>                 | <span data-ttu-id="0c15d-133">個人の名。</span><span class="sxs-lookup"><span data-stu-id="0c15d-133">The person's first name.</span></span>
| <span data-ttu-id="0c15d-134">**id**</span><span class="sxs-lookup"><span data-stu-id="0c15d-134">**id**</span></span>                        | <span data-ttu-id="0c15d-135">ディレクトリ内の個人またはグループの ID。</span><span class="sxs-lookup"><span data-stu-id="0c15d-135">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="0c15d-136">**lastName**</span><span class="sxs-lookup"><span data-stu-id="0c15d-136">**lastName**</span></span>                  | <span data-ttu-id="0c15d-137">個人の姓。</span><span class="sxs-lookup"><span data-stu-id="0c15d-137">The person's last name.</span></span>
| <span data-ttu-id="0c15d-138">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="0c15d-138">**mobilePhone**</span></span>               | <span data-ttu-id="0c15d-139">個人の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="0c15d-139">The person's mobile phone number.</span></span>
| <span data-ttu-id="0c15d-140">**name**</span><span class="sxs-lookup"><span data-stu-id="0c15d-140">**name**</span></span>                      | <span data-ttu-id="0c15d-141">個人の名前。</span><span class="sxs-lookup"><span data-stu-id="0c15d-141">The person's name.</span></span>
| <span data-ttu-id="0c15d-142">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="0c15d-142">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="0c15d-143">個人の名前、画像、その他の詳細。</span><span class="sxs-lookup"><span data-stu-id="0c15d-143">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="0c15d-144">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="0c15d-144">**nameWithPresence**</span></span>          | <span data-ttu-id="0c15d-145">既定値。</span><span class="sxs-lookup"><span data-stu-id="0c15d-145">Default.</span></span> <span data-ttu-id="0c15d-146">個人の名前とプレゼンス インジケーターのアイコン (連絡可能/通話中/その他)</span><span class="sxs-lookup"><span data-stu-id="0c15d-146">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="0c15d-147">**office**</span><span class="sxs-lookup"><span data-stu-id="0c15d-147">**office**</span></span>                    | <span data-ttu-id="0c15d-148">個人の会社の電話番号。</span><span class="sxs-lookup"><span data-stu-id="0c15d-148">The person's office number.</span></span>
| <span data-ttu-id="0c15d-149">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="0c15d-149">**pictureOnly36x36**</span></span>          | <span data-ttu-id="0c15d-150">36 x 36 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="0c15d-150">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="0c15d-151">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="0c15d-151">**pictureOnly48x48**</span></span>          | <span data-ttu-id="0c15d-152">48 x 48 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="0c15d-152">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="0c15d-153">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="0c15d-153">**pictureOnly72x72**</span></span>          | <span data-ttu-id="0c15d-154">72 x 72 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="0c15d-154">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="0c15d-155">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="0c15d-155">**sipAddress**</span></span>                | <span data-ttu-id="0c15d-156">個人の SIP アドレス。</span><span class="sxs-lookup"><span data-stu-id="0c15d-156">The person's sip address.</span></span>
| <span data-ttu-id="0c15d-157">**title**</span><span class="sxs-lookup"><span data-stu-id="0c15d-157">**title**</span></span>                     | <span data-ttu-id="0c15d-158">個人の組織内での役職。</span><span class="sxs-lookup"><span data-stu-id="0c15d-158">The person's title in the organization.</span></span>
| <span data-ttu-id="0c15d-159">**userName**</span><span class="sxs-lookup"><span data-stu-id="0c15d-159">**userName**</span></span>                  | <span data-ttu-id="0c15d-160">個人またはグループのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="0c15d-160">The person or group's user name.</span></span>
| <span data-ttu-id="0c15d-161">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="0c15d-161">**workEmail**</span></span>                 | <span data-ttu-id="0c15d-162">個人またはグループのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="0c15d-162">The person or group's email address.</span></span>
| <span data-ttu-id="0c15d-163">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="0c15d-163">**workPhone**</span></span>                 | <span data-ttu-id="0c15d-164">個人の勤務先電話番号。</span><span class="sxs-lookup"><span data-stu-id="0c15d-164">The person's work phone number.</span></span>

<span data-ttu-id="0c15d-165">注: その他の DisplayAs の種類が返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0c15d-165">Note: Additional DisplayAs types may be returned.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn",
  "suppressions": []
}
-->
