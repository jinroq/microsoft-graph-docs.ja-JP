---
title: termsAndConditions リソース タイプ
description: termsAndConditions エンティティは、特定の使用条件 (T&C) ポリシーのメタデータとコンテンツを表します。 T&C ポリシーのコンテンツは、ユーザーが Intune へ最初の登録を試みる際に表示されます。また、その後、管理者が再承認を必要とする編集の際にも表示されます。 それらを使用して、管理者は、デバイスを Intune に登録するためにユーザーが同意しなければならない規定を伝えることができます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9cce3e0d592b6be6f633910b8305a15ece1d30fa
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785413"
---
# <a name="termsandconditions-resource-type"></a><span data-ttu-id="3413b-105">termsAndConditions リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="3413b-105">termsAndConditions resource type</span></span>

> <span data-ttu-id="3413b-106">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3413b-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3413b-107">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3413b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3413b-108">termsAndConditions エンティティは、特定の使用条件 (T&C) ポリシーのメタデータとコンテンツを表します。</span><span class="sxs-lookup"><span data-stu-id="3413b-108">A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.</span></span> <span data-ttu-id="3413b-109">T&C ポリシーのコンテンツは、ユーザーが Intune へ最初の登録を試みる際に表示されます。また、その後、管理者が再承認を必要とする編集の際にも表示されます。</span><span class="sxs-lookup"><span data-stu-id="3413b-109">T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.</span></span> <span data-ttu-id="3413b-110">それらを使用して、管理者は、デバイスを Intune に登録するためにユーザーが同意しなければならない規定を伝えることができます。</span><span class="sxs-lookup"><span data-stu-id="3413b-110">They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="3413b-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="3413b-111">Methods</span></span>
|<span data-ttu-id="3413b-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="3413b-112">Method</span></span>|<span data-ttu-id="3413b-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3413b-113">Return Type</span></span>|<span data-ttu-id="3413b-114">説明</span><span class="sxs-lookup"><span data-stu-id="3413b-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3413b-115">termsAndConditionses のリスト</span><span class="sxs-lookup"><span data-stu-id="3413b-115">List termsAndConditionses</span></span>](../api/intune-companyterms-termsandconditions-list.md)|<span data-ttu-id="3413b-116">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3413b-116">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) collection</span></span>|<span data-ttu-id="3413b-117">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3413b-117">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>|
|[<span data-ttu-id="3413b-118">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3413b-118">Get termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-get.md)|[<span data-ttu-id="3413b-119">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3413b-119">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="3413b-120">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3413b-120">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="3413b-121">termsAndConditions の作成</span><span class="sxs-lookup"><span data-stu-id="3413b-121">Create termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-create.md)|[<span data-ttu-id="3413b-122">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3413b-122">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="3413b-123">新しい [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3413b-123">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="3413b-124">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3413b-124">Delete termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-delete.md)|<span data-ttu-id="3413b-125">なし</span><span class="sxs-lookup"><span data-stu-id="3413b-125">None</span></span>|<span data-ttu-id="3413b-126">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="3413b-126">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>|
|[<span data-ttu-id="3413b-127">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3413b-127">Update termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-update.md)|[<span data-ttu-id="3413b-128">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3413b-128">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="3413b-129">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3413b-129">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3413b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3413b-130">Properties</span></span>
|<span data-ttu-id="3413b-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3413b-131">Property</span></span>|<span data-ttu-id="3413b-132">型</span><span class="sxs-lookup"><span data-stu-id="3413b-132">Type</span></span>|<span data-ttu-id="3413b-133">説明</span><span class="sxs-lookup"><span data-stu-id="3413b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3413b-134">id</span><span class="sxs-lookup"><span data-stu-id="3413b-134">id</span></span>|<span data-ttu-id="3413b-135">文字列</span><span class="sxs-lookup"><span data-stu-id="3413b-135">String</span></span>|<span data-ttu-id="3413b-136">T&C ポリシーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="3413b-136">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="3413b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3413b-137">createdDateTime</span></span>|<span data-ttu-id="3413b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3413b-138">DateTimeOffset</span></span>|<span data-ttu-id="3413b-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3413b-139">DateTime the object was created.</span></span>|
|<span data-ttu-id="3413b-140">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3413b-140">modifiedDateTime</span></span>|<span data-ttu-id="3413b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3413b-141">DateTimeOffset</span></span>|<span data-ttu-id="3413b-142">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="3413b-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3413b-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3413b-143">lastModifiedDateTime</span></span>|<span data-ttu-id="3413b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3413b-144">DateTimeOffset</span></span>|<span data-ttu-id="3413b-145">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="3413b-145">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3413b-146">displayName</span><span class="sxs-lookup"><span data-stu-id="3413b-146">displayName</span></span>|<span data-ttu-id="3413b-147">String</span><span class="sxs-lookup"><span data-stu-id="3413b-147">String</span></span>|<span data-ttu-id="3413b-148">T&C ポリシー用に管理者が提供した名前。</span><span class="sxs-lookup"><span data-stu-id="3413b-148">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="3413b-149">説明</span><span class="sxs-lookup"><span data-stu-id="3413b-149">description</span></span>|<span data-ttu-id="3413b-150">String</span><span class="sxs-lookup"><span data-stu-id="3413b-150">String</span></span>|<span data-ttu-id="3413b-151">管理者が提供した T&C ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="3413b-151">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="3413b-152">title</span><span class="sxs-lookup"><span data-stu-id="3413b-152">title</span></span>|<span data-ttu-id="3413b-153">文字列</span><span class="sxs-lookup"><span data-stu-id="3413b-153">String</span></span>|<span data-ttu-id="3413b-154">管理者が提供した契約条件のタイトル。</span><span class="sxs-lookup"><span data-stu-id="3413b-154">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="3413b-155">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="3413b-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3413b-156">bodyText</span><span class="sxs-lookup"><span data-stu-id="3413b-156">bodyText</span></span>|<span data-ttu-id="3413b-157">文字列</span><span class="sxs-lookup"><span data-stu-id="3413b-157">String</span></span>|<span data-ttu-id="3413b-158">管理者が提供する契約条件の本文で、通常は条件そのものです。</span><span class="sxs-lookup"><span data-stu-id="3413b-158">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="3413b-159">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="3413b-159">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3413b-160">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="3413b-160">acceptanceStatement</span></span>|<span data-ttu-id="3413b-161">String</span><span class="sxs-lookup"><span data-stu-id="3413b-161">String</span></span>|<span data-ttu-id="3413b-162">使用条件に関する、管理者指定の説明内容です。通常は、T&C ポリシーに定められた使用条件を受け入れることの意味を記載します。</span><span class="sxs-lookup"><span data-stu-id="3413b-162">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="3413b-163">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="3413b-163">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3413b-164">version</span><span class="sxs-lookup"><span data-stu-id="3413b-164">version</span></span>|<span data-ttu-id="3413b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3413b-165">Int32</span></span>|<span data-ttu-id="3413b-166">条件の現行バージョンを示す整数。</span><span class="sxs-lookup"><span data-stu-id="3413b-166">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="3413b-167">管理者が使用条件を変更し、修正された T&C ポリシーを再承諾するようにユーザーに求めると、値が増加します。</span><span class="sxs-lookup"><span data-stu-id="3413b-167">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3413b-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3413b-168">Relationships</span></span>
|<span data-ttu-id="3413b-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3413b-169">Relationship</span></span>|<span data-ttu-id="3413b-170">型</span><span class="sxs-lookup"><span data-stu-id="3413b-170">Type</span></span>|<span data-ttu-id="3413b-171">説明</span><span class="sxs-lookup"><span data-stu-id="3413b-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3413b-172">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="3413b-172">groupAssignments</span></span>|<span data-ttu-id="3413b-173">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3413b-173">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="3413b-174">この T&C ポリシーのグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="3413b-174">The list of group assignments for this T&C policy.</span></span>|
|<span data-ttu-id="3413b-175">assignments</span><span class="sxs-lookup"><span data-stu-id="3413b-175">assignments</span></span>|<span data-ttu-id="3413b-176">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3413b-176">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="3413b-177">この T&C ポリシーの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="3413b-177">The list of assignments for this T&C policy.</span></span>|
|<span data-ttu-id="3413b-178">acceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="3413b-178">acceptanceStatuses</span></span>|<span data-ttu-id="3413b-179">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3413b-179">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="3413b-180">この T&C ポリシーの承諾状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="3413b-180">The list of acceptance statuses for this T&C policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3413b-181">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3413b-181">JSON Representation</span></span>
<span data-ttu-id="3413b-182">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3413b-182">Here is a JSON representation of the resource.</span></span>
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





