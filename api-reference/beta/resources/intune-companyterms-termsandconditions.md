---
title: termsAndConditions リソース タイプ
description: termsAndConditions エンティティは、特定の使用条件 (T&C) ポリシーのメタデータとコンテンツを表します。 T&C ポリシーのコンテンツは、ユーザーが Intune へ最初の登録を試みる際に表示されます。また、その後、管理者が再承認を必要とする編集の際にも表示されます。 それらを使用して、管理者は、デバイスを Intune に登録するためにユーザーが同意しなければならない規定を伝えることができます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 756b66776599b07ca95d54f75ca549a5319ef581
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989470"
---
# <a name="termsandconditions-resource-type"></a><span data-ttu-id="4fef9-105">termsAndConditions リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="4fef9-105">termsAndConditions resource type</span></span>

> <span data-ttu-id="4fef9-106">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fef9-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fef9-107">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4fef9-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fef9-108">termsAndConditions エンティティは、特定の使用条件 (T&C) ポリシーのメタデータとコンテンツを表します。</span><span class="sxs-lookup"><span data-stu-id="4fef9-108">A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.</span></span> <span data-ttu-id="4fef9-109">T&C ポリシーのコンテンツは、ユーザーが Intune へ最初の登録を試みる際に表示されます。また、その後、管理者が再承認を必要とする編集の際にも表示されます。</span><span class="sxs-lookup"><span data-stu-id="4fef9-109">T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.</span></span> <span data-ttu-id="4fef9-110">それらを使用して、管理者は、デバイスを Intune に登録するためにユーザーが同意しなければならない規定を伝えることができます。</span><span class="sxs-lookup"><span data-stu-id="4fef9-110">They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="4fef9-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fef9-111">Methods</span></span>
|<span data-ttu-id="4fef9-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fef9-112">Method</span></span>|<span data-ttu-id="4fef9-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4fef9-113">Return Type</span></span>|<span data-ttu-id="4fef9-114">説明</span><span class="sxs-lookup"><span data-stu-id="4fef9-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4fef9-115">List termsAndConditionses</span><span class="sxs-lookup"><span data-stu-id="4fef9-115">List termsAndConditionses</span></span>](../api/intune-companyterms-termsandconditions-list.md)|<span data-ttu-id="4fef9-116">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4fef9-116">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) collection</span></span>|<span data-ttu-id="4fef9-117">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4fef9-117">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>|
|[<span data-ttu-id="4fef9-118">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="4fef9-118">Get termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-get.md)|[<span data-ttu-id="4fef9-119">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="4fef9-119">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="4fef9-120">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4fef9-120">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="4fef9-121">Create termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="4fef9-121">Create termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-create.md)|[<span data-ttu-id="4fef9-122">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="4fef9-122">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="4fef9-123">新しい [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4fef9-123">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="4fef9-124">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="4fef9-124">Delete termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-delete.md)|<span data-ttu-id="4fef9-125">なし</span><span class="sxs-lookup"><span data-stu-id="4fef9-125">None</span></span>|<span data-ttu-id="4fef9-126">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="4fef9-126">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>|
|[<span data-ttu-id="4fef9-127">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="4fef9-127">Update termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-update.md)|[<span data-ttu-id="4fef9-128">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="4fef9-128">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="4fef9-129">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4fef9-129">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4fef9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fef9-130">Properties</span></span>
|<span data-ttu-id="4fef9-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fef9-131">Property</span></span>|<span data-ttu-id="4fef9-132">型</span><span class="sxs-lookup"><span data-stu-id="4fef9-132">Type</span></span>|<span data-ttu-id="4fef9-133">説明</span><span class="sxs-lookup"><span data-stu-id="4fef9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fef9-134">id</span><span class="sxs-lookup"><span data-stu-id="4fef9-134">id</span></span>|<span data-ttu-id="4fef9-135">文字列</span><span class="sxs-lookup"><span data-stu-id="4fef9-135">String</span></span>|<span data-ttu-id="4fef9-136">T&C ポリシーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="4fef9-136">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="4fef9-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4fef9-137">createdDateTime</span></span>|<span data-ttu-id="4fef9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fef9-138">DateTimeOffset</span></span>|<span data-ttu-id="4fef9-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4fef9-139">DateTime the object was created.</span></span>|
|<span data-ttu-id="4fef9-140">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4fef9-140">modifiedDateTime</span></span>|<span data-ttu-id="4fef9-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fef9-141">DateTimeOffset</span></span>|<span data-ttu-id="4fef9-142">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="4fef9-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="4fef9-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4fef9-143">lastModifiedDateTime</span></span>|<span data-ttu-id="4fef9-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fef9-144">DateTimeOffset</span></span>|<span data-ttu-id="4fef9-145">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="4fef9-145">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="4fef9-146">displayName</span><span class="sxs-lookup"><span data-stu-id="4fef9-146">displayName</span></span>|<span data-ttu-id="4fef9-147">文字列</span><span class="sxs-lookup"><span data-stu-id="4fef9-147">String</span></span>|<span data-ttu-id="4fef9-148">T&C ポリシー用に管理者が提供した名前。</span><span class="sxs-lookup"><span data-stu-id="4fef9-148">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="4fef9-149">description</span><span class="sxs-lookup"><span data-stu-id="4fef9-149">description</span></span>|<span data-ttu-id="4fef9-150">String</span><span class="sxs-lookup"><span data-stu-id="4fef9-150">String</span></span>|<span data-ttu-id="4fef9-151">管理者が提供した T&C ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="4fef9-151">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="4fef9-152">title</span><span class="sxs-lookup"><span data-stu-id="4fef9-152">title</span></span>|<span data-ttu-id="4fef9-153">String</span><span class="sxs-lookup"><span data-stu-id="4fef9-153">String</span></span>|<span data-ttu-id="4fef9-154">管理者が提供した契約条件のタイトル。</span><span class="sxs-lookup"><span data-stu-id="4fef9-154">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="4fef9-155">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="4fef9-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="4fef9-156">bodyText</span><span class="sxs-lookup"><span data-stu-id="4fef9-156">bodyText</span></span>|<span data-ttu-id="4fef9-157">String</span><span class="sxs-lookup"><span data-stu-id="4fef9-157">String</span></span>|<span data-ttu-id="4fef9-158">管理者が提供する契約条件の本文で、通常は条件そのものです。</span><span class="sxs-lookup"><span data-stu-id="4fef9-158">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="4fef9-159">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="4fef9-159">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="4fef9-160">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="4fef9-160">acceptanceStatement</span></span>|<span data-ttu-id="4fef9-161">String</span><span class="sxs-lookup"><span data-stu-id="4fef9-161">String</span></span>|<span data-ttu-id="4fef9-162">使用条件に関する、管理者指定の説明内容です。通常は、T&C ポリシーに定められた使用条件を受け入れることの意味を記載します。</span><span class="sxs-lookup"><span data-stu-id="4fef9-162">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="4fef9-163">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="4fef9-163">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="4fef9-164">version</span><span class="sxs-lookup"><span data-stu-id="4fef9-164">version</span></span>|<span data-ttu-id="4fef9-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4fef9-165">Int32</span></span>|<span data-ttu-id="4fef9-166">条件の現行バージョンを示す整数。</span><span class="sxs-lookup"><span data-stu-id="4fef9-166">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="4fef9-167">管理者が使用条件を変更し、修正された T&C ポリシーを再承諾するようにユーザーに求めると、値が増加します。</span><span class="sxs-lookup"><span data-stu-id="4fef9-167">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fef9-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4fef9-168">Relationships</span></span>
|<span data-ttu-id="4fef9-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4fef9-169">Relationship</span></span>|<span data-ttu-id="4fef9-170">型</span><span class="sxs-lookup"><span data-stu-id="4fef9-170">Type</span></span>|<span data-ttu-id="4fef9-171">説明</span><span class="sxs-lookup"><span data-stu-id="4fef9-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fef9-172">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="4fef9-172">groupAssignments</span></span>|<span data-ttu-id="4fef9-173">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4fef9-173">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="4fef9-174">この T&C ポリシーのグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="4fef9-174">The list of group assignments for this T&C policy.</span></span>|
|<span data-ttu-id="4fef9-175">assignments</span><span class="sxs-lookup"><span data-stu-id="4fef9-175">assignments</span></span>|<span data-ttu-id="4fef9-176">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4fef9-176">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="4fef9-177">この T&C ポリシーの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="4fef9-177">The list of assignments for this T&C policy.</span></span>|
|<span data-ttu-id="4fef9-178">acceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="4fef9-178">acceptanceStatuses</span></span>|<span data-ttu-id="4fef9-179">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4fef9-179">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="4fef9-180">この T&C ポリシーの承諾状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="4fef9-180">The list of acceptance statuses for this T&C policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4fef9-181">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4fef9-181">JSON Representation</span></span>
<span data-ttu-id="4fef9-182">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4fef9-182">Here is a JSON representation of the resource.</span></span>
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
  "modifiedDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": 1024
}
```





