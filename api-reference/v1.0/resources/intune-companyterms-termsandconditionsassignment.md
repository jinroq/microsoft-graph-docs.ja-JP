---
title: termsAndConditionsAssignment リソース タイプ
description: termsAndConditionsAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。 グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e4c8b7ac86f86f2b89bcd21a0576f68b823b9f6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523813"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="6fd02-104">termsAndConditionsAssignment リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="6fd02-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="6fd02-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6fd02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fd02-106">termsAndConditionsAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="6fd02-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="6fd02-107">グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6fd02-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="6fd02-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6fd02-108">Methods</span></span>
|<span data-ttu-id="6fd02-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6fd02-109">Method</span></span>|<span data-ttu-id="6fd02-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6fd02-110">Return Type</span></span>|<span data-ttu-id="6fd02-111">説明</span><span class="sxs-lookup"><span data-stu-id="6fd02-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6fd02-112">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="6fd02-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="6fd02-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6fd02-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="6fd02-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6fd02-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="6fd02-115">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="6fd02-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="6fd02-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="6fd02-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="6fd02-117">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6fd02-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="6fd02-118">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="6fd02-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="6fd02-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="6fd02-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="6fd02-120">新しい [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6fd02-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="6fd02-121">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="6fd02-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="6fd02-122">なし</span><span class="sxs-lookup"><span data-stu-id="6fd02-122">None</span></span>|<span data-ttu-id="6fd02-123">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6fd02-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="6fd02-124">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="6fd02-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="6fd02-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="6fd02-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="6fd02-126">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6fd02-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6fd02-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6fd02-127">Properties</span></span>
|<span data-ttu-id="6fd02-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6fd02-128">Property</span></span>|<span data-ttu-id="6fd02-129">型</span><span class="sxs-lookup"><span data-stu-id="6fd02-129">Type</span></span>|<span data-ttu-id="6fd02-130">説明</span><span class="sxs-lookup"><span data-stu-id="6fd02-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fd02-131">id</span><span class="sxs-lookup"><span data-stu-id="6fd02-131">id</span></span>|<span data-ttu-id="6fd02-132">String</span><span class="sxs-lookup"><span data-stu-id="6fd02-132">String</span></span>|<span data-ttu-id="6fd02-133">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6fd02-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="6fd02-134">target</span><span class="sxs-lookup"><span data-stu-id="6fd02-134">target</span></span>|[<span data-ttu-id="6fd02-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6fd02-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6fd02-136">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="6fd02-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fd02-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6fd02-137">Relationships</span></span>
<span data-ttu-id="6fd02-138">なし</span><span class="sxs-lookup"><span data-stu-id="6fd02-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fd02-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6fd02-139">JSON Representation</span></span>
<span data-ttu-id="6fd02-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6fd02-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



