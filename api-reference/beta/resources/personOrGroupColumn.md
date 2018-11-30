---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: 116e3a61938926ab75534bb2dc88363cc7d15196
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067417"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="bff14-102">PersonOrGroupColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bff14-102">PersonOrGroupColumn resource type</span></span>

> <span data-ttu-id="bff14-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bff14-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bff14-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bff14-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bff14-105">[columnDefinition](columndefinition.md) リソースの **PersonOrGroupColumn** は、列の値がディレクトリから選択した個人またはグループを表すことを示しています。</span><span class="sxs-lookup"><span data-stu-id="bff14-105">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bff14-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bff14-106">JSON representation</span></span>

<span data-ttu-id="bff14-107">以下は、**personOrGroupColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bff14-107">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="bff14-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bff14-108">Properties</span></span>

| <span data-ttu-id="bff14-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="bff14-109">Property name</span></span>              | <span data-ttu-id="bff14-110">型</span><span class="sxs-lookup"><span data-stu-id="bff14-110">Type</span></span>    | <span data-ttu-id="bff14-111">説明</span><span class="sxs-lookup"><span data-stu-id="bff14-111">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="bff14-112">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="bff14-112">**allowMultipleSelection**</span></span> | <span data-ttu-id="bff14-113">boolean</span><span class="sxs-lookup"><span data-stu-id="bff14-113">boolean</span></span> | <span data-ttu-id="bff14-114">ソースから複数の値を選択できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bff14-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="bff14-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="bff14-115">**displayAs**</span></span>              | <span data-ttu-id="bff14-116">文字列</span><span class="sxs-lookup"><span data-stu-id="bff14-116">string</span></span>  | <span data-ttu-id="bff14-117">選択された個人またはグループについての情報を表示する方法。</span><span class="sxs-lookup"><span data-stu-id="bff14-117">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="bff14-118">以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bff14-118">See below.</span></span>
| <span data-ttu-id="bff14-119">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="bff14-119">**chooseFromType**</span></span>         | <span data-ttu-id="bff14-120">文字列</span><span class="sxs-lookup"><span data-stu-id="bff14-120">string</span></span>  | <span data-ttu-id="bff14-121">個人のみ選択、または個人とグループの選択が可能かどうか。</span><span class="sxs-lookup"><span data-stu-id="bff14-121">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="bff14-122">`peopleAndGroups` または `peopleOnly` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="bff14-122">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="bff14-123">DisplayAs 値</span><span class="sxs-lookup"><span data-stu-id="bff14-123">DisplayAs values</span></span>

| <span data-ttu-id="bff14-124">DisplayAs 値</span><span class="sxs-lookup"><span data-stu-id="bff14-124">DisplayAs value</span></span>               | <span data-ttu-id="bff14-125">説明</span><span class="sxs-lookup"><span data-stu-id="bff14-125">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="bff14-126">**account**</span><span class="sxs-lookup"><span data-stu-id="bff14-126">**account**</span></span>                   | <span data-ttu-id="bff14-127">個人またはグループの、未加工の SharePoint エンコードの要求文字列 (たとえば </span><span class="sxs-lookup"><span data-stu-id="bff14-127">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="bff14-128">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="bff14-128">i:0#.f</span></span>|<span data-ttu-id="bff14-129">membership</span><span class="sxs-lookup"><span data-stu-id="bff14-129">membership</span></span>|<span data-ttu-id="bff14-130">jane@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="bff14-130">jane@contoso.com).</span></span>
| <span data-ttu-id="bff14-131">**department**</span><span class="sxs-lookup"><span data-stu-id="bff14-131">**department**</span></span>                | <span data-ttu-id="bff14-132">個人またはグループの部門。</span><span class="sxs-lookup"><span data-stu-id="bff14-132">The person or group's department.</span></span>
| <span data-ttu-id="bff14-133">**firstName**</span><span class="sxs-lookup"><span data-stu-id="bff14-133">**firstName**</span></span>                 | <span data-ttu-id="bff14-134">個人の名。</span><span class="sxs-lookup"><span data-stu-id="bff14-134">The person's first name.</span></span>
| <span data-ttu-id="bff14-135">**id**</span><span class="sxs-lookup"><span data-stu-id="bff14-135">**id**</span></span>                        | <span data-ttu-id="bff14-136">ディレクトリ内の個人またはグループの ID。</span><span class="sxs-lookup"><span data-stu-id="bff14-136">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="bff14-137">**lastName**</span><span class="sxs-lookup"><span data-stu-id="bff14-137">**lastName**</span></span>                  | <span data-ttu-id="bff14-138">個人の姓。</span><span class="sxs-lookup"><span data-stu-id="bff14-138">The person's last name.</span></span>
| <span data-ttu-id="bff14-139">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="bff14-139">**mobilePhone**</span></span>               | <span data-ttu-id="bff14-140">個人の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="bff14-140">The person's mobile phone number.</span></span>
| <span data-ttu-id="bff14-141">**name**</span><span class="sxs-lookup"><span data-stu-id="bff14-141">**name**</span></span>                      | <span data-ttu-id="bff14-142">個人の名前。</span><span class="sxs-lookup"><span data-stu-id="bff14-142">The person's name.</span></span>
| <span data-ttu-id="bff14-143">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="bff14-143">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="bff14-144">個人の名前、画像、その他の詳細。</span><span class="sxs-lookup"><span data-stu-id="bff14-144">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="bff14-145">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="bff14-145">**nameWithPresence**</span></span>          | <span data-ttu-id="bff14-146">既定値。</span><span class="sxs-lookup"><span data-stu-id="bff14-146">Default.</span></span> <span data-ttu-id="bff14-147">個人の名前とプレゼンス インジケーターのアイコン (連絡可能/通話中/その他)</span><span class="sxs-lookup"><span data-stu-id="bff14-147">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="bff14-148">**office**</span><span class="sxs-lookup"><span data-stu-id="bff14-148">**office**</span></span>                    | <span data-ttu-id="bff14-149">個人の会社の電話番号。</span><span class="sxs-lookup"><span data-stu-id="bff14-149">The person's office number.</span></span>
| <span data-ttu-id="bff14-150">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="bff14-150">**pictureOnly36x36**</span></span>          | <span data-ttu-id="bff14-151">36 x 36 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="bff14-151">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="bff14-152">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="bff14-152">**pictureOnly48x48**</span></span>          | <span data-ttu-id="bff14-153">48 x 48 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="bff14-153">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="bff14-154">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="bff14-154">**pictureOnly72x72**</span></span>          | <span data-ttu-id="bff14-155">72 x 72 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="bff14-155">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="bff14-156">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="bff14-156">**sipAddress**</span></span>                | <span data-ttu-id="bff14-157">個人の SIP アドレス。</span><span class="sxs-lookup"><span data-stu-id="bff14-157">The person's sip address.</span></span>
| <span data-ttu-id="bff14-158">**title**</span><span class="sxs-lookup"><span data-stu-id="bff14-158">**title**</span></span>                     | <span data-ttu-id="bff14-159">個人の組織内での役職。</span><span class="sxs-lookup"><span data-stu-id="bff14-159">The person's title in the organization.</span></span>
| <span data-ttu-id="bff14-160">**userName**</span><span class="sxs-lookup"><span data-stu-id="bff14-160">**userName**</span></span>                  | <span data-ttu-id="bff14-161">個人またはグループのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="bff14-161">The person or group's user name.</span></span>
| <span data-ttu-id="bff14-162">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="bff14-162">**workEmail**</span></span>                 | <span data-ttu-id="bff14-163">個人またはグループのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="bff14-163">The person or group's email address.</span></span>
| <span data-ttu-id="bff14-164">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="bff14-164">**workPhone**</span></span>                 | <span data-ttu-id="bff14-165">個人の勤務先電話番号。</span><span class="sxs-lookup"><span data-stu-id="bff14-165">The person's work phone number.</span></span>

<span data-ttu-id="bff14-166">注: その他の DisplayAs の種類が返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="bff14-166">Note: Additional DisplayAs types may be returned.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
