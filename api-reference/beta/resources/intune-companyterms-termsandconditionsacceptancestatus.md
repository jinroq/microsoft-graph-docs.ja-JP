---
title: termsAndConditionsAcceptanceStatus リソース タイプ
description: C) 特定のユーザーがポリシーです。 ポータル サイトへのアクセスを保持するには、ユーザーは最新バージョンの使用条件を承諾する必要があります。
author: tfitzmac
ms.openlocfilehash: 8e504796be7dbec303bab8691ed171abc80b9a45
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314638"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="59eba-104">termsAndConditionsAcceptanceStatus リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="59eba-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="59eba-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="59eba-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59eba-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59eba-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59eba-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="59eba-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59eba-108">termsAndConditionsAcceptanceStatus エンティティは、特定のユーザーによる特定の使用条件 (T&C) のポリシーの承諾状況を表します。</span><span class="sxs-lookup"><span data-stu-id="59eba-108">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="59eba-109">ポータル サイトへのアクセスを保持するには、ユーザーは最新バージョンの使用条件を承諾する必要があります。</span><span class="sxs-lookup"><span data-stu-id="59eba-109">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>
## <a name="methods"></a><span data-ttu-id="59eba-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="59eba-110">Methods</span></span>
|<span data-ttu-id="59eba-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="59eba-111">Method</span></span>|<span data-ttu-id="59eba-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="59eba-112">Return Type</span></span>|<span data-ttu-id="59eba-113">説明</span><span class="sxs-lookup"><span data-stu-id="59eba-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="59eba-114">List termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="59eba-114">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="59eba-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="59eba-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="59eba-116">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="59eba-116">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="59eba-117">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="59eba-117">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="59eba-118">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="59eba-118">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="59eba-119">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="59eba-119">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="59eba-120">Create termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="59eba-120">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="59eba-121">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="59eba-121">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="59eba-122">新しい [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="59eba-122">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="59eba-123">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="59eba-123">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="59eba-124">なし</span><span class="sxs-lookup"><span data-stu-id="59eba-124">None</span></span>|<span data-ttu-id="59eba-125">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="59eba-125">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="59eba-126">Update termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="59eba-126">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="59eba-127">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="59eba-127">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="59eba-128">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="59eba-128">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="59eba-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59eba-129">Properties</span></span>
|<span data-ttu-id="59eba-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59eba-130">Property</span></span>|<span data-ttu-id="59eba-131">種類</span><span class="sxs-lookup"><span data-stu-id="59eba-131">Type</span></span>|<span data-ttu-id="59eba-132">説明</span><span class="sxs-lookup"><span data-stu-id="59eba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59eba-133">ID</span><span class="sxs-lookup"><span data-stu-id="59eba-133">id</span></span>|<span data-ttu-id="59eba-134">String</span><span class="sxs-lookup"><span data-stu-id="59eba-134">String</span></span>|<span data-ttu-id="59eba-135">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="59eba-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="59eba-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="59eba-136">userDisplayName</span></span>|<span data-ttu-id="59eba-137">String</span><span class="sxs-lookup"><span data-stu-id="59eba-137">String</span></span>|<span data-ttu-id="59eba-138">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="59eba-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="59eba-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="59eba-139">acceptedVersion</span></span>|<span data-ttu-id="59eba-140">Int32</span><span class="sxs-lookup"><span data-stu-id="59eba-140">Int32</span></span>|<span data-ttu-id="59eba-141">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="59eba-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="59eba-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="59eba-142">acceptedDateTime</span></span>|<span data-ttu-id="59eba-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59eba-143">DateTimeOffset</span></span>|<span data-ttu-id="59eba-144">最後に使用条件がユーザーによって承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="59eba-144">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59eba-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59eba-145">Relationships</span></span>
|<span data-ttu-id="59eba-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59eba-146">Relationship</span></span>|<span data-ttu-id="59eba-147">型</span><span class="sxs-lookup"><span data-stu-id="59eba-147">Type</span></span>|<span data-ttu-id="59eba-148">説明</span><span class="sxs-lookup"><span data-stu-id="59eba-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59eba-149">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="59eba-149">termsAndConditions</span></span>|[<span data-ttu-id="59eba-150">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="59eba-150">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="59eba-151">割り当てられた使用条件へのナビゲーション リンク。</span><span class="sxs-lookup"><span data-stu-id="59eba-151">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59eba-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59eba-152">JSON Representation</span></span>
<span data-ttu-id="59eba-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59eba-153">Here is a JSON representation of the resource.</span></span>
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





