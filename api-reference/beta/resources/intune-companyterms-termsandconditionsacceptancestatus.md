---
title: termsAndConditionsAcceptanceStatus リソース タイプ
description: termsAndConditionsAcceptanceStatus エンティティは、特定のユーザーによる特定の使用条件 (T&C) のポリシーの承諾状況を表します。 ポータル サイトへのアクセスを保持するには、ユーザーは最新バージョンの使用条件を承諾する必要があります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 967e64dc4182dc78abf85ad1b3dfd6a398f82dac
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987706"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="83c1a-104">termsAndConditionsAcceptanceStatus リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="83c1a-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="83c1a-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83c1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83c1a-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="83c1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83c1a-107">termsAndConditionsAcceptanceStatus エンティティは、特定のユーザーによる特定の使用条件 (T&C) のポリシーの承諾状況を表します。</span><span class="sxs-lookup"><span data-stu-id="83c1a-107">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="83c1a-108">ポータル サイトへのアクセスを保持するには、ユーザーは最新バージョンの使用条件を承諾する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83c1a-108">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>

## <a name="methods"></a><span data-ttu-id="83c1a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="83c1a-109">Methods</span></span>
|<span data-ttu-id="83c1a-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="83c1a-110">Method</span></span>|<span data-ttu-id="83c1a-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="83c1a-111">Return Type</span></span>|<span data-ttu-id="83c1a-112">説明</span><span class="sxs-lookup"><span data-stu-id="83c1a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="83c1a-113">List termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="83c1a-113">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="83c1a-114">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="83c1a-114">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="83c1a-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="83c1a-115">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="83c1a-116">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="83c1a-116">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="83c1a-117">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="83c1a-117">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="83c1a-118">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="83c1a-118">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="83c1a-119">Create termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="83c1a-119">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="83c1a-120">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="83c1a-120">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="83c1a-121">新しい [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="83c1a-121">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="83c1a-122">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="83c1a-122">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="83c1a-123">なし</span><span class="sxs-lookup"><span data-stu-id="83c1a-123">None</span></span>|<span data-ttu-id="83c1a-124">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="83c1a-124">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="83c1a-125">Update termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="83c1a-125">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="83c1a-126">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="83c1a-126">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="83c1a-127">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="83c1a-127">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="83c1a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83c1a-128">Properties</span></span>
|<span data-ttu-id="83c1a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83c1a-129">Property</span></span>|<span data-ttu-id="83c1a-130">型</span><span class="sxs-lookup"><span data-stu-id="83c1a-130">Type</span></span>|<span data-ttu-id="83c1a-131">説明</span><span class="sxs-lookup"><span data-stu-id="83c1a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83c1a-132">id</span><span class="sxs-lookup"><span data-stu-id="83c1a-132">id</span></span>|<span data-ttu-id="83c1a-133">文字列</span><span class="sxs-lookup"><span data-stu-id="83c1a-133">String</span></span>|<span data-ttu-id="83c1a-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="83c1a-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="83c1a-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="83c1a-135">userDisplayName</span></span>|<span data-ttu-id="83c1a-136">String</span><span class="sxs-lookup"><span data-stu-id="83c1a-136">String</span></span>|<span data-ttu-id="83c1a-137">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="83c1a-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="83c1a-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="83c1a-138">acceptedVersion</span></span>|<span data-ttu-id="83c1a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="83c1a-139">Int32</span></span>|<span data-ttu-id="83c1a-140">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="83c1a-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="83c1a-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="83c1a-141">acceptedDateTime</span></span>|<span data-ttu-id="83c1a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83c1a-142">DateTimeOffset</span></span>|<span data-ttu-id="83c1a-143">最後に使用条件がユーザーによって承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="83c1a-143">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83c1a-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="83c1a-144">Relationships</span></span>
|<span data-ttu-id="83c1a-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="83c1a-145">Relationship</span></span>|<span data-ttu-id="83c1a-146">型</span><span class="sxs-lookup"><span data-stu-id="83c1a-146">Type</span></span>|<span data-ttu-id="83c1a-147">説明</span><span class="sxs-lookup"><span data-stu-id="83c1a-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83c1a-148">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="83c1a-148">termsAndConditions</span></span>|[<span data-ttu-id="83c1a-149">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="83c1a-149">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="83c1a-150">割り当てられた使用条件へのナビゲーション リンク。</span><span class="sxs-lookup"><span data-stu-id="83c1a-150">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83c1a-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="83c1a-151">JSON Representation</span></span>
<span data-ttu-id="83c1a-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="83c1a-152">Here is a JSON representation of the resource.</span></span>
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





