---
title: termsAndConditionsAssignment リソース タイプ
description: termsAndConditionsAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。 グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2de08d2bc90061ed4096a9a010b332872eb36ef
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422027"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="67e46-104">termsAndConditionsAssignment リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="67e46-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="67e46-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="67e46-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="67e46-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67e46-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67e46-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="67e46-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67e46-108">termsAndConditionsAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="67e46-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="67e46-109">グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="67e46-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="67e46-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="67e46-110">Methods</span></span>
|<span data-ttu-id="67e46-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="67e46-111">Method</span></span>|<span data-ttu-id="67e46-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="67e46-112">Return Type</span></span>|<span data-ttu-id="67e46-113">説明</span><span class="sxs-lookup"><span data-stu-id="67e46-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="67e46-114">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="67e46-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="67e46-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="67e46-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="67e46-116">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="67e46-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="67e46-117">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="67e46-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="67e46-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="67e46-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="67e46-119">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="67e46-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="67e46-120">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="67e46-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="67e46-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="67e46-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="67e46-122">新しい [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="67e46-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="67e46-123">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="67e46-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="67e46-124">なし</span><span class="sxs-lookup"><span data-stu-id="67e46-124">None</span></span>|<span data-ttu-id="67e46-125">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="67e46-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="67e46-126">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="67e46-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="67e46-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="67e46-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="67e46-128">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="67e46-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="67e46-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67e46-129">Properties</span></span>
|<span data-ttu-id="67e46-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67e46-130">Property</span></span>|<span data-ttu-id="67e46-131">型</span><span class="sxs-lookup"><span data-stu-id="67e46-131">Type</span></span>|<span data-ttu-id="67e46-132">説明</span><span class="sxs-lookup"><span data-stu-id="67e46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67e46-133">id</span><span class="sxs-lookup"><span data-stu-id="67e46-133">id</span></span>|<span data-ttu-id="67e46-134">String</span><span class="sxs-lookup"><span data-stu-id="67e46-134">String</span></span>|<span data-ttu-id="67e46-135">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="67e46-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="67e46-136">target</span><span class="sxs-lookup"><span data-stu-id="67e46-136">target</span></span>|[<span data-ttu-id="67e46-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="67e46-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="67e46-138">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="67e46-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67e46-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="67e46-139">Relationships</span></span>
<span data-ttu-id="67e46-140">なし</span><span class="sxs-lookup"><span data-stu-id="67e46-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67e46-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="67e46-141">JSON Representation</span></span>
<span data-ttu-id="67e46-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="67e46-142">Here is a JSON representation of the resource.</span></span>
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




