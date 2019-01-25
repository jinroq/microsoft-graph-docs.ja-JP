---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a3136d7c5b9563999eb9b21a9235317afdaeb63e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519298"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="a0268-102">PersonOrGroupColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a0268-102">PersonOrGroupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0268-103">[columnDefinition](columndefinition.md) リソースの **PersonOrGroupColumn** は、列の値がディレクトリから選択した個人またはグループを表すことを示しています。</span><span class="sxs-lookup"><span data-stu-id="a0268-103">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0268-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a0268-104">JSON representation</span></span>

<span data-ttu-id="a0268-105">以下は、**personOrGroupColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a0268-105">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="a0268-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0268-106">Properties</span></span>

| <span data-ttu-id="a0268-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="a0268-107">Property name</span></span>              | <span data-ttu-id="a0268-108">種類</span><span class="sxs-lookup"><span data-stu-id="a0268-108">Type</span></span>    | <span data-ttu-id="a0268-109">説明</span><span class="sxs-lookup"><span data-stu-id="a0268-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="a0268-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="a0268-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="a0268-111">boolean</span><span class="sxs-lookup"><span data-stu-id="a0268-111">boolean</span></span> | <span data-ttu-id="a0268-112">ソースから複数の値を選択できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a0268-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="a0268-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="a0268-113">**displayAs**</span></span>              | <span data-ttu-id="a0268-114">string</span><span class="sxs-lookup"><span data-stu-id="a0268-114">string</span></span>  | <span data-ttu-id="a0268-115">選択された個人またはグループについての情報を表示する方法。</span><span class="sxs-lookup"><span data-stu-id="a0268-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="a0268-116">以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a0268-116">See below.</span></span>
| <span data-ttu-id="a0268-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="a0268-117">**chooseFromType**</span></span>         | <span data-ttu-id="a0268-118">string</span><span class="sxs-lookup"><span data-stu-id="a0268-118">string</span></span>  | <span data-ttu-id="a0268-119">個人のみ選択、または個人とグループの選択が可能かどうか。</span><span class="sxs-lookup"><span data-stu-id="a0268-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="a0268-120">`peopleAndGroups` または `peopleOnly` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="a0268-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="a0268-121">DisplayAs 値</span><span class="sxs-lookup"><span data-stu-id="a0268-121">DisplayAs values</span></span>

| <span data-ttu-id="a0268-122">DisplayAs 値</span><span class="sxs-lookup"><span data-stu-id="a0268-122">DisplayAs value</span></span>               | <span data-ttu-id="a0268-123">説明</span><span class="sxs-lookup"><span data-stu-id="a0268-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="a0268-124">**account**</span><span class="sxs-lookup"><span data-stu-id="a0268-124">**account**</span></span>                   | <span data-ttu-id="a0268-125">個人またはグループの、未加工の SharePoint エンコードの要求文字列 (たとえば </span><span class="sxs-lookup"><span data-stu-id="a0268-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="a0268-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="a0268-126">i:0#.f</span></span>|<span data-ttu-id="a0268-127">membership</span><span class="sxs-lookup"><span data-stu-id="a0268-127">membership</span></span>|<span data-ttu-id="a0268-128">jane@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="a0268-128">jane@contoso.com).</span></span>
| <span data-ttu-id="a0268-129">**department**</span><span class="sxs-lookup"><span data-stu-id="a0268-129">**department**</span></span>                | <span data-ttu-id="a0268-130">個人またはグループの部門。</span><span class="sxs-lookup"><span data-stu-id="a0268-130">The person or group's department.</span></span>
| <span data-ttu-id="a0268-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="a0268-131">**firstName**</span></span>                 | <span data-ttu-id="a0268-132">個人の名。</span><span class="sxs-lookup"><span data-stu-id="a0268-132">The person's first name.</span></span>
| <span data-ttu-id="a0268-133">**id**</span><span class="sxs-lookup"><span data-stu-id="a0268-133">**id**</span></span>                        | <span data-ttu-id="a0268-134">ディレクトリ内の個人またはグループの ID。</span><span class="sxs-lookup"><span data-stu-id="a0268-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="a0268-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="a0268-135">**lastName**</span></span>                  | <span data-ttu-id="a0268-136">個人の姓。</span><span class="sxs-lookup"><span data-stu-id="a0268-136">The person's last name.</span></span>
| <span data-ttu-id="a0268-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="a0268-137">**mobilePhone**</span></span>               | <span data-ttu-id="a0268-138">個人の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="a0268-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="a0268-139">**name**</span><span class="sxs-lookup"><span data-stu-id="a0268-139">**name**</span></span>                      | <span data-ttu-id="a0268-140">個人の名前。</span><span class="sxs-lookup"><span data-stu-id="a0268-140">The person's name.</span></span>
| <span data-ttu-id="a0268-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="a0268-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="a0268-142">個人の名前、画像、その他の詳細。</span><span class="sxs-lookup"><span data-stu-id="a0268-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="a0268-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="a0268-143">**nameWithPresence**</span></span>          | <span data-ttu-id="a0268-144">既定値。</span><span class="sxs-lookup"><span data-stu-id="a0268-144">Default.</span></span> <span data-ttu-id="a0268-145">個人の名前とプレゼンス インジケーターのアイコン (連絡可能/通話中/その他)</span><span class="sxs-lookup"><span data-stu-id="a0268-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="a0268-146">**office**</span><span class="sxs-lookup"><span data-stu-id="a0268-146">**office**</span></span>                    | <span data-ttu-id="a0268-147">個人の会社の電話番号。</span><span class="sxs-lookup"><span data-stu-id="a0268-147">The person's office number.</span></span>
| <span data-ttu-id="a0268-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="a0268-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="a0268-149">36 x 36 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="a0268-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="a0268-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="a0268-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="a0268-151">48 x 48 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="a0268-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="a0268-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="a0268-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="a0268-153">72 x 72 ピクセルの正方形で囲まれた個人の画像。</span><span class="sxs-lookup"><span data-stu-id="a0268-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="a0268-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="a0268-154">**sipAddress**</span></span>                | <span data-ttu-id="a0268-155">個人の SIP アドレス。</span><span class="sxs-lookup"><span data-stu-id="a0268-155">The person's sip address.</span></span>
| <span data-ttu-id="a0268-156">**title**</span><span class="sxs-lookup"><span data-stu-id="a0268-156">**title**</span></span>                     | <span data-ttu-id="a0268-157">個人の組織内での役職。</span><span class="sxs-lookup"><span data-stu-id="a0268-157">The person's title in the organization.</span></span>
| <span data-ttu-id="a0268-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="a0268-158">**userName**</span></span>                  | <span data-ttu-id="a0268-159">個人またはグループのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="a0268-159">The person or group's user name.</span></span>
| <span data-ttu-id="a0268-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="a0268-160">**workEmail**</span></span>                 | <span data-ttu-id="a0268-161">個人またはグループのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="a0268-161">The person or group's email address.</span></span>
| <span data-ttu-id="a0268-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="a0268-162">**workPhone**</span></span>                 | <span data-ttu-id="a0268-163">個人の勤務先電話番号。</span><span class="sxs-lookup"><span data-stu-id="a0268-163">The person's work phone number.</span></span>

<span data-ttu-id="a0268-164">注: その他の DisplayAs の種類が返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a0268-164">Note: Additional DisplayAs types may be returned.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/personOrGroupColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
