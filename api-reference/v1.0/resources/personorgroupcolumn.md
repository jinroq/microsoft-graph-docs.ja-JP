---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
description: columnDefinition リソースの PersonOrGroupColumn は、列の値がディレクトリから選択した個人またはグループを表すことを示しています。
doc_type: resourcePageType
ms.openlocfilehash: d8ce31e7eb044e588f73afefb2b370e161fa7cdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035519"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="bf0a9-103">PersonOrGroupColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf0a9-103">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="bf0a9-104">[columnDefinition](columndefinition.md) リソースの **PersonOrGroupColumn** は、列の値がディレクトリから選択した個人またはグループを表すことを示しています。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-104">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf0a9-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf0a9-105">JSON representation</span></span>

<span data-ttu-id="bf0a9-106">以下は、**personOrGroupColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-106">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="bf0a9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf0a9-107">Properties</span></span>

| <span data-ttu-id="bf0a9-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="bf0a9-108">Property name</span></span>              | <span data-ttu-id="bf0a9-109">種類</span><span class="sxs-lookup"><span data-stu-id="bf0a9-109">Type</span></span>    | <span data-ttu-id="bf0a9-110">説明</span><span class="sxs-lookup"><span data-stu-id="bf0a9-110">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="bf0a9-111">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-111">**allowMultipleSelection**</span></span> | <span data-ttu-id="bf0a9-112">boolean</span><span class="sxs-lookup"><span data-stu-id="bf0a9-112">boolean</span></span> | <span data-ttu-id="bf0a9-113">ソースから複数の値を選択できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-113">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="bf0a9-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-114">**displayAs**</span></span>              | <span data-ttu-id="bf0a9-115">string</span><span class="sxs-lookup"><span data-stu-id="bf0a9-115">string</span></span>  | <span data-ttu-id="bf0a9-116">選択された個人またはグループについての情報を表示する方法。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-116">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="bf0a9-117">以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-117">See below.</span></span>
| <span data-ttu-id="bf0a9-118">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-118">**chooseFromType**</span></span>         | <span data-ttu-id="bf0a9-119">string</span><span class="sxs-lookup"><span data-stu-id="bf0a9-119">string</span></span>  | <span data-ttu-id="bf0a9-120">個人のみ選択、または個人とグループの選択が可能かどうか。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-120">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="bf0a9-121">`peopleAndGroups` または `peopleOnly` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-121">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="bf0a9-122">DisplayAs オプション</span><span class="sxs-lookup"><span data-stu-id="bf0a9-122">DisplayAs options</span></span>

| <span data-ttu-id="bf0a9-123">DisplayAs 値</span><span class="sxs-lookup"><span data-stu-id="bf0a9-123">DisplayAs value</span></span>               | <span data-ttu-id="bf0a9-124">説明</span><span class="sxs-lookup"><span data-stu-id="bf0a9-124">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="bf0a9-125">**account**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-125">**account**</span></span>                   | <span data-ttu-id="bf0a9-126">個人またはグループの、未加工の SharePoint エンコードの要求文字列 (たとえば </span><span class="sxs-lookup"><span data-stu-id="bf0a9-126">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="bf0a9-127">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="bf0a9-127">i:0#.f</span></span>|<span data-ttu-id="bf0a9-128">membership</span><span class="sxs-lookup"><span data-stu-id="bf0a9-128">membership</span></span>|<span data-ttu-id="bf0a9-129">jane@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-129">jane@contoso.com).</span></span>
| <span data-ttu-id="bf0a9-130">**department**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-130">**department**</span></span>                | <span data-ttu-id="bf0a9-131">個人またはグループの部門。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-131">The person or group's department.</span></span>
| <span data-ttu-id="bf0a9-132">**firstName**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-132">**firstName**</span></span>                 | <span data-ttu-id="bf0a9-133">個人の名。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-133">The person's first name.</span></span>
| <span data-ttu-id="bf0a9-134">**id**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-134">**id**</span></span>                        | <span data-ttu-id="bf0a9-135">ディレクトリ内の個人またはグループの ID。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-135">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="bf0a9-136">**lastName**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-136">**lastName**</span></span>                  | <span data-ttu-id="bf0a9-137">個人の姓。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-137">The person's last name.</span></span>
| <span data-ttu-id="bf0a9-138">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-138">**mobilePhone**</span></span>               | <span data-ttu-id="bf0a9-139">個人の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-139">The person's mobile phone number.</span></span>
| <span data-ttu-id="bf0a9-140">**name**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-140">**name**</span></span>                      | <span data-ttu-id="bf0a9-141">個人の名前。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-141">The person's name.</span></span>
| <span data-ttu-id="bf0a9-142">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-142">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="bf0a9-143">個人の名前、画像、その他の詳細。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-143">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="bf0a9-144">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-144">**nameWithPresence**</span></span>          | <span data-ttu-id="bf0a9-145">既定値。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-145">Default.</span></span> <span data-ttu-id="bf0a9-146">個人の名前とプレゼンス インジケーターのアイコン (連絡可能/通話中/その他)</span><span class="sxs-lookup"><span data-stu-id="bf0a9-146">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="bf0a9-147">**office**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-147">**office**</span></span>                    | <span data-ttu-id="bf0a9-148">個人の会社の電話番号。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-148">The person's office number.</span></span>
| <span data-ttu-id="bf0a9-149">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-149">**pictureOnly36x36**</span></span>          | <span data-ttu-id="bf0a9-150">36 x 36 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-150">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="bf0a9-151">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-151">**pictureOnly48x48**</span></span>          | <span data-ttu-id="bf0a9-152">48 x 48 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-152">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="bf0a9-153">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-153">**pictureOnly72x72**</span></span>          | <span data-ttu-id="bf0a9-154">72 x 72 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-154">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="bf0a9-155">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-155">**sipAddress**</span></span>                | <span data-ttu-id="bf0a9-156">個人の SIP アドレス。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-156">The person's sip address.</span></span>
| <span data-ttu-id="bf0a9-157">**title**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-157">**title**</span></span>                     | <span data-ttu-id="bf0a9-158">個人の組織内での役職。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-158">The person's title in the organization.</span></span>
| <span data-ttu-id="bf0a9-159">**userName**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-159">**userName**</span></span>                  | <span data-ttu-id="bf0a9-160">個人またはグループのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-160">The person or group's user name.</span></span>
| <span data-ttu-id="bf0a9-161">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-161">**workEmail**</span></span>                 | <span data-ttu-id="bf0a9-162">個人またはグループのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-162">The person or group's email address.</span></span>
| <span data-ttu-id="bf0a9-163">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="bf0a9-163">**workPhone**</span></span>                 | <span data-ttu-id="bf0a9-164">個人の勤務先電話番号。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-164">The person's work phone number.</span></span>

<span data-ttu-id="bf0a9-165">注: その他の DisplayAs の種類が返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="bf0a9-165">Note: Additional DisplayAs types may be returned.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(peopleAndGroups,peopleOnly) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(account,contentType,created,department,...) are in resource, but () are in table"
  ],
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
