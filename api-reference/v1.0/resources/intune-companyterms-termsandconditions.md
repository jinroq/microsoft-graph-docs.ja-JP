---
title: termsAndConditions リソース タイプ
description: termsAndConditions エンティティは、特定の使用条件 (T&C) ポリシーのメタデータとコンテンツを表します。 T&C ポリシーのコンテンツは、ユーザーが Intune へ最初の登録を試みる際に表示されます。また、その後、管理者が再承認を必要とする編集の際にも表示されます。 それらを使用して、管理者は、デバイスを Intune に登録するためにユーザーが同意しなければならない規定を伝えることができます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: be4cf9b5145a6e5ee320e82f33ec2f67a70829a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031991"
---
# <a name="termsandconditions-resource-type"></a><span data-ttu-id="da923-105">termsAndConditions リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="da923-105">termsAndConditions resource type</span></span>

> <span data-ttu-id="da923-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="da923-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da923-107">termsAndConditions エンティティは、特定の使用条件 (T&C) ポリシーのメタデータとコンテンツを表します。</span><span class="sxs-lookup"><span data-stu-id="da923-107">A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.</span></span> <span data-ttu-id="da923-108">T&C ポリシーのコンテンツは、ユーザーが Intune へ最初の登録を試みる際に表示されます。また、その後、管理者が再承認を必要とする編集の際にも表示されます。</span><span class="sxs-lookup"><span data-stu-id="da923-108">T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.</span></span> <span data-ttu-id="da923-109">それらを使用して、管理者は、デバイスを Intune に登録するためにユーザーが同意しなければならない規定を伝えることができます。</span><span class="sxs-lookup"><span data-stu-id="da923-109">They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="da923-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="da923-110">Methods</span></span>
|<span data-ttu-id="da923-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="da923-111">Method</span></span>|<span data-ttu-id="da923-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="da923-112">Return Type</span></span>|<span data-ttu-id="da923-113">説明</span><span class="sxs-lookup"><span data-stu-id="da923-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="da923-114">List termsAndConditionses</span><span class="sxs-lookup"><span data-stu-id="da923-114">List termsAndConditionses</span></span>](../api/intune-companyterms-termsandconditions-list.md)|<span data-ttu-id="da923-115">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="da923-115">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) collection</span></span>|<span data-ttu-id="da923-116">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="da923-116">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>|
|[<span data-ttu-id="da923-117">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="da923-117">Get termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-get.md)|[<span data-ttu-id="da923-118">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="da923-118">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="da923-119">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="da923-119">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="da923-120">Create termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="da923-120">Create termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-create.md)|[<span data-ttu-id="da923-121">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="da923-121">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="da923-122">新しい [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="da923-122">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="da923-123">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="da923-123">Delete termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-delete.md)|<span data-ttu-id="da923-124">なし</span><span class="sxs-lookup"><span data-stu-id="da923-124">None</span></span>|<span data-ttu-id="da923-125">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="da923-125">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>|
|[<span data-ttu-id="da923-126">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="da923-126">Update termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-update.md)|[<span data-ttu-id="da923-127">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="da923-127">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="da923-128">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="da923-128">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="da923-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da923-129">Properties</span></span>
|<span data-ttu-id="da923-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da923-130">Property</span></span>|<span data-ttu-id="da923-131">型</span><span class="sxs-lookup"><span data-stu-id="da923-131">Type</span></span>|<span data-ttu-id="da923-132">説明</span><span class="sxs-lookup"><span data-stu-id="da923-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da923-133">id</span><span class="sxs-lookup"><span data-stu-id="da923-133">id</span></span>|<span data-ttu-id="da923-134">文字列</span><span class="sxs-lookup"><span data-stu-id="da923-134">String</span></span>|<span data-ttu-id="da923-135">T&C ポリシーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="da923-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="da923-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da923-136">createdDateTime</span></span>|<span data-ttu-id="da923-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da923-137">DateTimeOffset</span></span>|<span data-ttu-id="da923-138">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="da923-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="da923-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da923-139">lastModifiedDateTime</span></span>|<span data-ttu-id="da923-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da923-140">DateTimeOffset</span></span>|<span data-ttu-id="da923-141">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="da923-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="da923-142">displayName</span><span class="sxs-lookup"><span data-stu-id="da923-142">displayName</span></span>|<span data-ttu-id="da923-143">文字列</span><span class="sxs-lookup"><span data-stu-id="da923-143">String</span></span>|<span data-ttu-id="da923-144">T&C ポリシー用に管理者が提供した名前。</span><span class="sxs-lookup"><span data-stu-id="da923-144">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="da923-145">description</span><span class="sxs-lookup"><span data-stu-id="da923-145">description</span></span>|<span data-ttu-id="da923-146">String</span><span class="sxs-lookup"><span data-stu-id="da923-146">String</span></span>|<span data-ttu-id="da923-147">管理者が提供した T&C ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="da923-147">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="da923-148">title</span><span class="sxs-lookup"><span data-stu-id="da923-148">title</span></span>|<span data-ttu-id="da923-149">String</span><span class="sxs-lookup"><span data-stu-id="da923-149">String</span></span>|<span data-ttu-id="da923-150">管理者が提供した契約条件のタイトル。</span><span class="sxs-lookup"><span data-stu-id="da923-150">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="da923-151">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="da923-151">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="da923-152">bodyText</span><span class="sxs-lookup"><span data-stu-id="da923-152">bodyText</span></span>|<span data-ttu-id="da923-153">String</span><span class="sxs-lookup"><span data-stu-id="da923-153">String</span></span>|<span data-ttu-id="da923-154">管理者が提供する契約条件の本文で、通常は条件そのものです。</span><span class="sxs-lookup"><span data-stu-id="da923-154">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="da923-155">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="da923-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="da923-156">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="da923-156">acceptanceStatement</span></span>|<span data-ttu-id="da923-157">String</span><span class="sxs-lookup"><span data-stu-id="da923-157">String</span></span>|<span data-ttu-id="da923-158">使用条件に関する、管理者指定の説明内容です。通常は、T&C ポリシーに定められた使用条件を受け入れることの意味を記載します。</span><span class="sxs-lookup"><span data-stu-id="da923-158">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="da923-159">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="da923-159">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="da923-160">version</span><span class="sxs-lookup"><span data-stu-id="da923-160">version</span></span>|<span data-ttu-id="da923-161">Int32</span><span class="sxs-lookup"><span data-stu-id="da923-161">Int32</span></span>|<span data-ttu-id="da923-162">条件の現行バージョンを示す整数。</span><span class="sxs-lookup"><span data-stu-id="da923-162">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="da923-163">管理者が使用条件を変更し、修正された T&C ポリシーを再承諾するようにユーザーに求めると、値が増加します。</span><span class="sxs-lookup"><span data-stu-id="da923-163">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da923-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="da923-164">Relationships</span></span>
|<span data-ttu-id="da923-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="da923-165">Relationship</span></span>|<span data-ttu-id="da923-166">型</span><span class="sxs-lookup"><span data-stu-id="da923-166">Type</span></span>|<span data-ttu-id="da923-167">説明</span><span class="sxs-lookup"><span data-stu-id="da923-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da923-168">assignments</span><span class="sxs-lookup"><span data-stu-id="da923-168">assignments</span></span>|<span data-ttu-id="da923-169">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="da923-169">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="da923-170">この T&C ポリシーの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="da923-170">The list of assignments for this T&C policy.</span></span>|
|<span data-ttu-id="da923-171">acceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="da923-171">acceptanceStatuses</span></span>|<span data-ttu-id="da923-172">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="da923-172">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="da923-173">この T&C ポリシーの承諾状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="da923-173">The list of acceptance statuses for this T&C policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="da923-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="da923-174">JSON Representation</span></span>
<span data-ttu-id="da923-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="da923-175">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": 1024
}
```



