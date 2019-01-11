---
title: termsAndConditionsAcceptanceStatus リソース タイプ
description: C) 特定のユーザーがポリシーです。 ポータル サイトへのアクセスを保持するには、ユーザーは最新バージョンの使用条件を承諾する必要があります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 17d76be4db1f790d00fb90322307ff04152291be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849393"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="eef77-104">termsAndConditionsAcceptanceStatus リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="eef77-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="eef77-105">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="eef77-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eef77-106">termsAndConditionsAcceptanceStatus エンティティは、特定のユーザーによる特定の使用条件 (T&C) のポリシーの承諾状況を表します。</span><span class="sxs-lookup"><span data-stu-id="eef77-106">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="eef77-107">ポータル サイトへのアクセスを保持するには、ユーザーは最新バージョンの使用条件を承諾する必要があります。</span><span class="sxs-lookup"><span data-stu-id="eef77-107">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>
## <a name="methods"></a><span data-ttu-id="eef77-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="eef77-108">Methods</span></span>
|<span data-ttu-id="eef77-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="eef77-109">Method</span></span>|<span data-ttu-id="eef77-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="eef77-110">Return Type</span></span>|<span data-ttu-id="eef77-111">説明</span><span class="sxs-lookup"><span data-stu-id="eef77-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eef77-112">List termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="eef77-112">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="eef77-113">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="eef77-113">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="eef77-114">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="eef77-114">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="eef77-115">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="eef77-115">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="eef77-116">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="eef77-116">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="eef77-117">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="eef77-117">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="eef77-118">Create termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="eef77-118">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="eef77-119">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="eef77-119">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="eef77-120">新しい [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="eef77-120">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="eef77-121">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="eef77-121">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="eef77-122">なし</span><span class="sxs-lookup"><span data-stu-id="eef77-122">None</span></span>|<span data-ttu-id="eef77-123">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="eef77-123">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="eef77-124">Update termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="eef77-124">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="eef77-125">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="eef77-125">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="eef77-126">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="eef77-126">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="eef77-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eef77-127">Properties</span></span>
|<span data-ttu-id="eef77-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eef77-128">Property</span></span>|<span data-ttu-id="eef77-129">種類</span><span class="sxs-lookup"><span data-stu-id="eef77-129">Type</span></span>|<span data-ttu-id="eef77-130">説明</span><span class="sxs-lookup"><span data-stu-id="eef77-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eef77-131">ID</span><span class="sxs-lookup"><span data-stu-id="eef77-131">id</span></span>|<span data-ttu-id="eef77-132">String</span><span class="sxs-lookup"><span data-stu-id="eef77-132">String</span></span>|<span data-ttu-id="eef77-133">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="eef77-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="eef77-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="eef77-134">userDisplayName</span></span>|<span data-ttu-id="eef77-135">String</span><span class="sxs-lookup"><span data-stu-id="eef77-135">String</span></span>|<span data-ttu-id="eef77-136">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="eef77-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="eef77-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="eef77-137">acceptedVersion</span></span>|<span data-ttu-id="eef77-138">Int32</span><span class="sxs-lookup"><span data-stu-id="eef77-138">Int32</span></span>|<span data-ttu-id="eef77-139">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="eef77-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="eef77-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="eef77-140">acceptedDateTime</span></span>|<span data-ttu-id="eef77-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eef77-141">DateTimeOffset</span></span>|<span data-ttu-id="eef77-142">最後に使用条件がユーザーによって承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="eef77-142">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eef77-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eef77-143">Relationships</span></span>
|<span data-ttu-id="eef77-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eef77-144">Relationship</span></span>|<span data-ttu-id="eef77-145">型</span><span class="sxs-lookup"><span data-stu-id="eef77-145">Type</span></span>|<span data-ttu-id="eef77-146">説明</span><span class="sxs-lookup"><span data-stu-id="eef77-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eef77-147">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="eef77-147">termsAndConditions</span></span>|[<span data-ttu-id="eef77-148">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="eef77-148">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="eef77-149">割り当てられた使用条件へのナビゲーション リンク。</span><span class="sxs-lookup"><span data-stu-id="eef77-149">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eef77-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eef77-150">JSON Representation</span></span>
<span data-ttu-id="eef77-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eef77-151">Here is a JSON representation of the resource.</span></span>
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



