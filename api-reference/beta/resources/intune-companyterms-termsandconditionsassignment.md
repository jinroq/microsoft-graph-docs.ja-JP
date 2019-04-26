---
title: termsAndConditionsAssignment リソース タイプ
description: termsAndConditionsAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。 グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b6bff777bfaf093d1148a584cc8524069304b70
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557986"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="83cbf-104">termsAndConditionsAssignment リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="83cbf-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="83cbf-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83cbf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83cbf-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="83cbf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83cbf-107">termsAndConditionsAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="83cbf-107">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="83cbf-108">グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83cbf-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="83cbf-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="83cbf-109">Methods</span></span>
|<span data-ttu-id="83cbf-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="83cbf-110">Method</span></span>|<span data-ttu-id="83cbf-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="83cbf-111">Return Type</span></span>|<span data-ttu-id="83cbf-112">説明</span><span class="sxs-lookup"><span data-stu-id="83cbf-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="83cbf-113">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="83cbf-113">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="83cbf-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="83cbf-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="83cbf-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="83cbf-115">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="83cbf-116">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="83cbf-116">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="83cbf-117">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="83cbf-117">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="83cbf-118">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="83cbf-118">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="83cbf-119">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="83cbf-119">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="83cbf-120">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="83cbf-120">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="83cbf-121">新しい [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="83cbf-121">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="83cbf-122">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="83cbf-122">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="83cbf-123">なし</span><span class="sxs-lookup"><span data-stu-id="83cbf-123">None</span></span>|<span data-ttu-id="83cbf-124">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="83cbf-124">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="83cbf-125">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="83cbf-125">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="83cbf-126">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="83cbf-126">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="83cbf-127">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="83cbf-127">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="83cbf-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83cbf-128">Properties</span></span>
|<span data-ttu-id="83cbf-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83cbf-129">Property</span></span>|<span data-ttu-id="83cbf-130">型</span><span class="sxs-lookup"><span data-stu-id="83cbf-130">Type</span></span>|<span data-ttu-id="83cbf-131">説明</span><span class="sxs-lookup"><span data-stu-id="83cbf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83cbf-132">id</span><span class="sxs-lookup"><span data-stu-id="83cbf-132">id</span></span>|<span data-ttu-id="83cbf-133">String</span><span class="sxs-lookup"><span data-stu-id="83cbf-133">String</span></span>|<span data-ttu-id="83cbf-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="83cbf-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="83cbf-135">target</span><span class="sxs-lookup"><span data-stu-id="83cbf-135">target</span></span>|[<span data-ttu-id="83cbf-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="83cbf-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="83cbf-137">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="83cbf-137">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83cbf-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="83cbf-138">Relationships</span></span>
<span data-ttu-id="83cbf-139">なし</span><span class="sxs-lookup"><span data-stu-id="83cbf-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83cbf-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="83cbf-140">JSON Representation</span></span>
<span data-ttu-id="83cbf-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="83cbf-141">Here is a JSON representation of the resource.</span></span>
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





