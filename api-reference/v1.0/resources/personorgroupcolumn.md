---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: b0c6eab7d2111870192a4ed6c30c1cbd72e4163e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022974"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="603ef-102">PersonOrGroupColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="603ef-102">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="603ef-103">[columnDefinition](columndefinition.md) リソースの **PersonOrGroupColumn** は、列の値がディレクトリから選択した個人またはグループを表すことを示しています。</span><span class="sxs-lookup"><span data-stu-id="603ef-103">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="603ef-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="603ef-104">JSON representation</span></span>

<span data-ttu-id="603ef-105">以下は、**personOrGroupColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="603ef-105">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="603ef-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="603ef-106">Properties</span></span>

| <span data-ttu-id="603ef-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="603ef-107">Property name</span></span>              | <span data-ttu-id="603ef-108">種類</span><span class="sxs-lookup"><span data-stu-id="603ef-108">Type</span></span>    | <span data-ttu-id="603ef-109">説明</span><span class="sxs-lookup"><span data-stu-id="603ef-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="603ef-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="603ef-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="603ef-111">boolean</span><span class="sxs-lookup"><span data-stu-id="603ef-111">boolean</span></span> | <span data-ttu-id="603ef-112">ソースから複数の値を選択できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="603ef-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="603ef-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="603ef-113">**displayAs**</span></span>              | <span data-ttu-id="603ef-114">string</span><span class="sxs-lookup"><span data-stu-id="603ef-114">string</span></span>  | <span data-ttu-id="603ef-115">選択された個人またはグループについての情報を表示する方法。</span><span class="sxs-lookup"><span data-stu-id="603ef-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="603ef-116">以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="603ef-116">See below.</span></span>
| <span data-ttu-id="603ef-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="603ef-117">**chooseFromType**</span></span>         | <span data-ttu-id="603ef-118">string</span><span class="sxs-lookup"><span data-stu-id="603ef-118">string</span></span>  | <span data-ttu-id="603ef-119">個人のみ選択、または個人とグループの選択が可能かどうか。</span><span class="sxs-lookup"><span data-stu-id="603ef-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="603ef-120">`peopleAndGroups` または `peopleOnly` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="603ef-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="603ef-121">DisplayAs オプション</span><span class="sxs-lookup"><span data-stu-id="603ef-121">DisplayAs options</span></span>

| <span data-ttu-id="603ef-122">DisplayAs 値</span><span class="sxs-lookup"><span data-stu-id="603ef-122">DisplayAs value</span></span>               | <span data-ttu-id="603ef-123">説明</span><span class="sxs-lookup"><span data-stu-id="603ef-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="603ef-124">**account**</span><span class="sxs-lookup"><span data-stu-id="603ef-124">**account**</span></span>                   | <span data-ttu-id="603ef-125">個人またはグループの、未加工の SharePoint エンコードの要求文字列 (たとえば </span><span class="sxs-lookup"><span data-stu-id="603ef-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="603ef-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="603ef-126">i:0#.f</span></span>|<span data-ttu-id="603ef-127">membership</span><span class="sxs-lookup"><span data-stu-id="603ef-127">membership</span></span>|<span data-ttu-id="603ef-128">jane@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="603ef-128">jane@contoso.com).</span></span>
| <span data-ttu-id="603ef-129">**department**</span><span class="sxs-lookup"><span data-stu-id="603ef-129">**department**</span></span>                | <span data-ttu-id="603ef-130">個人またはグループの部門。</span><span class="sxs-lookup"><span data-stu-id="603ef-130">The person or group's department.</span></span>
| <span data-ttu-id="603ef-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="603ef-131">**firstName**</span></span>                 | <span data-ttu-id="603ef-132">個人の名。</span><span class="sxs-lookup"><span data-stu-id="603ef-132">The person's first name.</span></span>
| <span data-ttu-id="603ef-133">**id**</span><span class="sxs-lookup"><span data-stu-id="603ef-133">**id**</span></span>                        | <span data-ttu-id="603ef-134">ディレクトリ内の個人またはグループの ID。</span><span class="sxs-lookup"><span data-stu-id="603ef-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="603ef-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="603ef-135">**lastName**</span></span>                  | <span data-ttu-id="603ef-136">個人の姓。</span><span class="sxs-lookup"><span data-stu-id="603ef-136">The person's last name.</span></span>
| <span data-ttu-id="603ef-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="603ef-137">**mobilePhone**</span></span>               | <span data-ttu-id="603ef-138">個人の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="603ef-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="603ef-139">**name**</span><span class="sxs-lookup"><span data-stu-id="603ef-139">**name**</span></span>                      | <span data-ttu-id="603ef-140">個人の名前。</span><span class="sxs-lookup"><span data-stu-id="603ef-140">The person's name.</span></span>
| <span data-ttu-id="603ef-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="603ef-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="603ef-142">個人の名前、画像、その他の詳細。</span><span class="sxs-lookup"><span data-stu-id="603ef-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="603ef-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="603ef-143">**nameWithPresence**</span></span>          | <span data-ttu-id="603ef-144">既定値。</span><span class="sxs-lookup"><span data-stu-id="603ef-144">Default.</span></span> <span data-ttu-id="603ef-145">個人の名前とプレゼンス インジケーターのアイコン (連絡可能/通話中/その他)</span><span class="sxs-lookup"><span data-stu-id="603ef-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="603ef-146">**office**</span><span class="sxs-lookup"><span data-stu-id="603ef-146">**office**</span></span>                    | <span data-ttu-id="603ef-147">個人の会社の電話番号。</span><span class="sxs-lookup"><span data-stu-id="603ef-147">The person's office number.</span></span>
| <span data-ttu-id="603ef-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="603ef-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="603ef-149">36 x 36 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="603ef-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="603ef-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="603ef-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="603ef-151">48 x 48 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="603ef-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="603ef-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="603ef-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="603ef-153">72 x 72 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="603ef-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="603ef-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="603ef-154">**sipAddress**</span></span>                | <span data-ttu-id="603ef-155">個人の SIP アドレス。</span><span class="sxs-lookup"><span data-stu-id="603ef-155">The person's sip address.</span></span>
| <span data-ttu-id="603ef-156">**title**</span><span class="sxs-lookup"><span data-stu-id="603ef-156">**title**</span></span>                     | <span data-ttu-id="603ef-157">個人の組織内での役職。</span><span class="sxs-lookup"><span data-stu-id="603ef-157">The person's title in the organization.</span></span>
| <span data-ttu-id="603ef-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="603ef-158">**userName**</span></span>                  | <span data-ttu-id="603ef-159">個人またはグループのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="603ef-159">The person or group's user name.</span></span>
| <span data-ttu-id="603ef-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="603ef-160">**workEmail**</span></span>                 | <span data-ttu-id="603ef-161">個人またはグループのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="603ef-161">The person or group's email address.</span></span>
| <span data-ttu-id="603ef-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="603ef-162">**workPhone**</span></span>                 | <span data-ttu-id="603ef-163">個人の勤務先電話番号。</span><span class="sxs-lookup"><span data-stu-id="603ef-163">The person's work phone number.</span></span>

<span data-ttu-id="603ef-164">注: その他の DisplayAs の種類が返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="603ef-164">Note: Additional DisplayAs types may be returned.</span></span>

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
