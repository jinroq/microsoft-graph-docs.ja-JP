---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 5ff8d61a2796edd615a66416b4f8f4d6d565909a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985452"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="8b9cb-102">PersonOrGroupColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b9cb-102">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="8b9cb-103">[columnDefinition](columndefinition.md) リソースの **PersonOrGroupColumn** は、列の値がディレクトリから選択した個人またはグループを表すことを示しています。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-103">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b9cb-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b9cb-104">JSON representation</span></span>

<span data-ttu-id="8b9cb-105">以下は、**personOrGroupColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-105">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="8b9cb-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b9cb-106">Properties</span></span>

| <span data-ttu-id="8b9cb-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="8b9cb-107">Property name</span></span>              | <span data-ttu-id="8b9cb-108">種類</span><span class="sxs-lookup"><span data-stu-id="8b9cb-108">Type</span></span>    | <span data-ttu-id="8b9cb-109">説明</span><span class="sxs-lookup"><span data-stu-id="8b9cb-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="8b9cb-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="8b9cb-111">boolean</span><span class="sxs-lookup"><span data-stu-id="8b9cb-111">boolean</span></span> | <span data-ttu-id="8b9cb-112">ソースから複数の値を選択できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="8b9cb-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-113">**displayAs**</span></span>              | <span data-ttu-id="8b9cb-114">string</span><span class="sxs-lookup"><span data-stu-id="8b9cb-114">string</span></span>  | <span data-ttu-id="8b9cb-115">選択された個人またはグループについての情報を表示する方法。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="8b9cb-116">以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-116">See below.</span></span>
| <span data-ttu-id="8b9cb-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-117">**chooseFromType**</span></span>         | <span data-ttu-id="8b9cb-118">string</span><span class="sxs-lookup"><span data-stu-id="8b9cb-118">string</span></span>  | <span data-ttu-id="8b9cb-119">個人のみ選択、または個人とグループの選択が可能かどうか。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="8b9cb-120">`peopleAndGroups` または `peopleOnly` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="8b9cb-121">DisplayAs オプション</span><span class="sxs-lookup"><span data-stu-id="8b9cb-121">DisplayAs options</span></span>

| <span data-ttu-id="8b9cb-122">DisplayAs 値</span><span class="sxs-lookup"><span data-stu-id="8b9cb-122">DisplayAs value</span></span>               | <span data-ttu-id="8b9cb-123">説明</span><span class="sxs-lookup"><span data-stu-id="8b9cb-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="8b9cb-124">**account**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-124">**account**</span></span>                   | <span data-ttu-id="8b9cb-125">個人またはグループの、未加工の SharePoint エンコードの要求文字列 (たとえば </span><span class="sxs-lookup"><span data-stu-id="8b9cb-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="8b9cb-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="8b9cb-126">i:0#.f</span></span>|<span data-ttu-id="8b9cb-127">membership</span><span class="sxs-lookup"><span data-stu-id="8b9cb-127">membership</span></span>|<span data-ttu-id="8b9cb-128">jane@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-128">jane@contoso.com).</span></span>
| <span data-ttu-id="8b9cb-129">**department**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-129">**department**</span></span>                | <span data-ttu-id="8b9cb-130">個人またはグループの部門。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-130">The person or group's department.</span></span>
| <span data-ttu-id="8b9cb-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-131">**firstName**</span></span>                 | <span data-ttu-id="8b9cb-132">個人の名。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-132">The person's first name.</span></span>
| <span data-ttu-id="8b9cb-133">**id**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-133">**id**</span></span>                        | <span data-ttu-id="8b9cb-134">ディレクトリ内の個人またはグループの ID。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="8b9cb-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-135">**lastName**</span></span>                  | <span data-ttu-id="8b9cb-136">個人の姓。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-136">The person's last name.</span></span>
| <span data-ttu-id="8b9cb-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-137">**mobilePhone**</span></span>               | <span data-ttu-id="8b9cb-138">個人の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="8b9cb-139">**name**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-139">**name**</span></span>                      | <span data-ttu-id="8b9cb-140">個人の名前。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-140">The person's name.</span></span>
| <span data-ttu-id="8b9cb-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="8b9cb-142">個人の名前、画像、その他の詳細。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="8b9cb-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-143">**nameWithPresence**</span></span>          | <span data-ttu-id="8b9cb-144">既定値。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-144">Default.</span></span> <span data-ttu-id="8b9cb-145">個人の名前とプレゼンス インジケーターのアイコン (連絡可能/通話中/その他)</span><span class="sxs-lookup"><span data-stu-id="8b9cb-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="8b9cb-146">**office**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-146">**office**</span></span>                    | <span data-ttu-id="8b9cb-147">個人の会社の電話番号。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-147">The person's office number.</span></span>
| <span data-ttu-id="8b9cb-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="8b9cb-149">36 x 36 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="8b9cb-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="8b9cb-151">48 x 48 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="8b9cb-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="8b9cb-153">72 x 72 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="8b9cb-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-154">**sipAddress**</span></span>                | <span data-ttu-id="8b9cb-155">個人の SIP アドレス。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-155">The person's sip address.</span></span>
| <span data-ttu-id="8b9cb-156">**title**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-156">**title**</span></span>                     | <span data-ttu-id="8b9cb-157">個人の組織内での役職。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-157">The person's title in the organization.</span></span>
| <span data-ttu-id="8b9cb-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-158">**userName**</span></span>                  | <span data-ttu-id="8b9cb-159">個人またはグループのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-159">The person or group's user name.</span></span>
| <span data-ttu-id="8b9cb-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-160">**workEmail**</span></span>                 | <span data-ttu-id="8b9cb-161">個人またはグループのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-161">The person or group's email address.</span></span>
| <span data-ttu-id="8b9cb-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-162">**workPhone**</span></span>                 | <span data-ttu-id="8b9cb-163">個人の勤務先電話番号。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-163">The person's work phone number.</span></span>

<span data-ttu-id="8b9cb-164">注: その他の DisplayAs の種類が返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="8b9cb-164">Note: Additional DisplayAs types may be returned.</span></span>

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
