---
title: termsAndConditionsAcceptanceStatus リソース タイプ
description: termsAndConditionsAcceptanceStatus エンティティは、特定のユーザーによる特定の使用条件 (T&C) のポリシーの承諾状況を表します。 ポータル サイトへのアクセスを保持するには、ユーザーは最新バージョンの使用条件を承諾する必要があります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9e222e760f4f0971ea21a904312629517a7104f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028750"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="ba29f-104">termsAndConditionsAcceptanceStatus リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="ba29f-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="ba29f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba29f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba29f-106">termsAndConditionsAcceptanceStatus エンティティは、特定のユーザーによる特定の使用条件 (T&C) のポリシーの承諾状況を表します。</span><span class="sxs-lookup"><span data-stu-id="ba29f-106">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="ba29f-107">ポータル サイトへのアクセスを保持するには、ユーザーは最新バージョンの使用条件を承諾する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ba29f-107">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>

## <a name="methods"></a><span data-ttu-id="ba29f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ba29f-108">Methods</span></span>
|<span data-ttu-id="ba29f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ba29f-109">Method</span></span>|<span data-ttu-id="ba29f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ba29f-110">Return Type</span></span>|<span data-ttu-id="ba29f-111">説明</span><span class="sxs-lookup"><span data-stu-id="ba29f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ba29f-112">List termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="ba29f-112">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="ba29f-113">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ba29f-113">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="ba29f-114">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ba29f-114">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="ba29f-115">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ba29f-115">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="ba29f-116">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ba29f-116">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="ba29f-117">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ba29f-117">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="ba29f-118">Create termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ba29f-118">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="ba29f-119">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ba29f-119">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="ba29f-120">新しい [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ba29f-120">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="ba29f-121">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ba29f-121">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="ba29f-122">なし</span><span class="sxs-lookup"><span data-stu-id="ba29f-122">None</span></span>|<span data-ttu-id="ba29f-123">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="ba29f-123">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="ba29f-124">Update termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ba29f-124">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="ba29f-125">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ba29f-125">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="ba29f-126">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ba29f-126">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ba29f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba29f-127">Properties</span></span>
|<span data-ttu-id="ba29f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba29f-128">Property</span></span>|<span data-ttu-id="ba29f-129">型</span><span class="sxs-lookup"><span data-stu-id="ba29f-129">Type</span></span>|<span data-ttu-id="ba29f-130">説明</span><span class="sxs-lookup"><span data-stu-id="ba29f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba29f-131">id</span><span class="sxs-lookup"><span data-stu-id="ba29f-131">id</span></span>|<span data-ttu-id="ba29f-132">文字列</span><span class="sxs-lookup"><span data-stu-id="ba29f-132">String</span></span>|<span data-ttu-id="ba29f-133">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ba29f-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ba29f-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ba29f-134">userDisplayName</span></span>|<span data-ttu-id="ba29f-135">String</span><span class="sxs-lookup"><span data-stu-id="ba29f-135">String</span></span>|<span data-ttu-id="ba29f-136">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="ba29f-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="ba29f-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="ba29f-137">acceptedVersion</span></span>|<span data-ttu-id="ba29f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="ba29f-138">Int32</span></span>|<span data-ttu-id="ba29f-139">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="ba29f-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="ba29f-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba29f-140">acceptedDateTime</span></span>|<span data-ttu-id="ba29f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba29f-141">DateTimeOffset</span></span>|<span data-ttu-id="ba29f-142">最後に使用条件がユーザーによって承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ba29f-142">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba29f-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ba29f-143">Relationships</span></span>
|<span data-ttu-id="ba29f-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ba29f-144">Relationship</span></span>|<span data-ttu-id="ba29f-145">型</span><span class="sxs-lookup"><span data-stu-id="ba29f-145">Type</span></span>|<span data-ttu-id="ba29f-146">説明</span><span class="sxs-lookup"><span data-stu-id="ba29f-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba29f-147">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ba29f-147">termsAndConditions</span></span>|[<span data-ttu-id="ba29f-148">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ba29f-148">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="ba29f-149">割り当てられた使用条件へのナビゲーション リンク。</span><span class="sxs-lookup"><span data-stu-id="ba29f-149">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba29f-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba29f-150">JSON Representation</span></span>
<span data-ttu-id="ba29f-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ba29f-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```



