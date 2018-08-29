---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: 37c324ddb1863e3e589e7d17ea60bd879e50771f
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267557"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="b93c1-102">PersonOrGroupColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b93c1-102">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="b93c1-103">[columnDefinition](columnDefinition.md) リソースの **PersonOrGroupColumn** は、列の値がディレクトリから選択した個人またはグループを表すことを示しています。</span><span class="sxs-lookup"><span data-stu-id="b93c1-103">The **personOrGroupColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b93c1-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b93c1-104">JSON representation</span></span>

<span data-ttu-id="b93c1-105">以下は、**personOrGroupColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b93c1-105">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="b93c1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b93c1-106">Properties</span></span>

| <span data-ttu-id="b93c1-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="b93c1-107">Property name</span></span>              | <span data-ttu-id="b93c1-108">型</span><span class="sxs-lookup"><span data-stu-id="b93c1-108">Type</span></span>    | <span data-ttu-id="b93c1-109">説明</span><span class="sxs-lookup"><span data-stu-id="b93c1-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="b93c1-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="b93c1-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="b93c1-111">ブール値</span><span class="sxs-lookup"><span data-stu-id="b93c1-111">boolean</span></span> | <span data-ttu-id="b93c1-112">ソースから複数の値を選択できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b93c1-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="b93c1-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="b93c1-113">**displayAs**</span></span>              | <span data-ttu-id="b93c1-114">文字列</span><span class="sxs-lookup"><span data-stu-id="b93c1-114">string</span></span>  | <span data-ttu-id="b93c1-115">選択された個人またはグループについての情報を表示する方法。</span><span class="sxs-lookup"><span data-stu-id="b93c1-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="b93c1-116">以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b93c1-116">See below.</span></span>
| <span data-ttu-id="b93c1-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="b93c1-117">**chooseFromType**</span></span>         | <span data-ttu-id="b93c1-118">文字列</span><span class="sxs-lookup"><span data-stu-id="b93c1-118">string</span></span>  | <span data-ttu-id="b93c1-119">個人のみ選択、または個人とグループの選択が可能かどうか。</span><span class="sxs-lookup"><span data-stu-id="b93c1-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="b93c1-120">`peopleAndGroups` または `peopleOnly` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="b93c1-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="b93c1-121">DisplayAs オプション</span><span class="sxs-lookup"><span data-stu-id="b93c1-121">DisplayAs options</span></span>

| <span data-ttu-id="b93c1-122">DisplayAs 値</span><span class="sxs-lookup"><span data-stu-id="b93c1-122">DisplayAs value</span></span>               | <span data-ttu-id="b93c1-123">説明</span><span class="sxs-lookup"><span data-stu-id="b93c1-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="b93c1-124">**アカウント**</span><span class="sxs-lookup"><span data-stu-id="b93c1-124">**account**</span></span>                   | <span data-ttu-id="b93c1-125">個人またはグループの、未加工の SharePoint エンコードの要求文字列 (たとえば</span><span class="sxs-lookup"><span data-stu-id="b93c1-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="b93c1-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="b93c1-126">i:0#.f</span></span>|<span data-ttu-id="b93c1-127">メンバーシップ</span><span class="sxs-lookup"><span data-stu-id="b93c1-127">membership</span></span>|<span data-ttu-id="b93c1-128">jane@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="b93c1-128">jane@contoso.com).</span></span>
| <span data-ttu-id="b93c1-129">**department**</span><span class="sxs-lookup"><span data-stu-id="b93c1-129">**department**</span></span>                | <span data-ttu-id="b93c1-130">個人またはグループの部門。</span><span class="sxs-lookup"><span data-stu-id="b93c1-130">The person or group's department.</span></span>
| <span data-ttu-id="b93c1-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="b93c1-131">**firstName**</span></span>                 | <span data-ttu-id="b93c1-132">個人の名。</span><span class="sxs-lookup"><span data-stu-id="b93c1-132">The person's first name.</span></span>
| <span data-ttu-id="b93c1-133">**id**</span><span class="sxs-lookup"><span data-stu-id="b93c1-133">**id**</span></span>                        | <span data-ttu-id="b93c1-134">ディレクトリ内の個人またはグループの ID。</span><span class="sxs-lookup"><span data-stu-id="b93c1-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="b93c1-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="b93c1-135">**lastName**</span></span>                  | <span data-ttu-id="b93c1-136">個人の姓。</span><span class="sxs-lookup"><span data-stu-id="b93c1-136">The person's last name.</span></span>
| <span data-ttu-id="b93c1-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="b93c1-137">**mobilePhone**</span></span>               | <span data-ttu-id="b93c1-138">個人の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="b93c1-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="b93c1-139">**name**</span><span class="sxs-lookup"><span data-stu-id="b93c1-139">**name**</span></span>                      | <span data-ttu-id="b93c1-140">個人の名前。</span><span class="sxs-lookup"><span data-stu-id="b93c1-140">The person's name.</span></span>
| <span data-ttu-id="b93c1-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="b93c1-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="b93c1-142">個人の名前、画像、その他の詳細。</span><span class="sxs-lookup"><span data-stu-id="b93c1-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="b93c1-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="b93c1-143">**nameWithPresence**</span></span>          | <span data-ttu-id="b93c1-144">既定値。</span><span class="sxs-lookup"><span data-stu-id="b93c1-144">Default.</span></span> <span data-ttu-id="b93c1-145">個人の名前とプレゼンス インジケーターのアイコン (連絡可能/通話中/その他)</span><span class="sxs-lookup"><span data-stu-id="b93c1-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="b93c1-146">**office**</span><span class="sxs-lookup"><span data-stu-id="b93c1-146">**office**</span></span>                    | <span data-ttu-id="b93c1-147">個人の会社の電話番号。</span><span class="sxs-lookup"><span data-stu-id="b93c1-147">The person's office number.</span></span>
| <span data-ttu-id="b93c1-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="b93c1-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="b93c1-149">36 x 36 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="b93c1-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="b93c1-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="b93c1-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="b93c1-151">48 x 48 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="b93c1-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="b93c1-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="b93c1-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="b93c1-153">72 x 72 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="b93c1-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="b93c1-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="b93c1-154">**sipAddress**</span></span>                | <span data-ttu-id="b93c1-155">個人の SIP アドレス。</span><span class="sxs-lookup"><span data-stu-id="b93c1-155">The person's sip address.</span></span>
| <span data-ttu-id="b93c1-156">**title**</span><span class="sxs-lookup"><span data-stu-id="b93c1-156">**title**</span></span>                     | <span data-ttu-id="b93c1-157">個人の組織内での役職。</span><span class="sxs-lookup"><span data-stu-id="b93c1-157">The person's title in the organization.</span></span>
| <span data-ttu-id="b93c1-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="b93c1-158">**userName**</span></span>                  | <span data-ttu-id="b93c1-159">個人またはグループのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="b93c1-159">The person or group's user name.</span></span>
| <span data-ttu-id="b93c1-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="b93c1-160">**workEmail**</span></span>                 | <span data-ttu-id="b93c1-161">個人またはグループのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="b93c1-161">The person or group's email address.</span></span>
| <span data-ttu-id="b93c1-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="b93c1-162">**workPhone**</span></span>                 | <span data-ttu-id="b93c1-163">個人の勤務先電話番号。</span><span class="sxs-lookup"><span data-stu-id="b93c1-163">The person's work phone number.</span></span>

<span data-ttu-id="b93c1-164">注: その他の DisplayAs の種類が返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b93c1-164">Note: Additional DisplayAs types may be returned.</span></span>

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
