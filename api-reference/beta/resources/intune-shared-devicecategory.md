---
title: deviceCategory リソースの種類
description: これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。 レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。
ms.openlocfilehash: ccbd8d464f733c44cff3000f60b047142d6fb987
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070123"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="72c71-104">deviceCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="72c71-104">deviceCategory resource type</span></span>

> <span data-ttu-id="72c71-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="72c71-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72c71-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72c71-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72c71-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="72c71-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72c71-108">カテゴリのデバイスは、デバイスを分類する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="72c71-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="72c71-109">カテゴリのデバイスを使用すると、会社の管理者は、会社に意味のある一意のカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="72c71-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="72c71-110">これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="72c71-110"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="72c71-111">レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="72c71-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="72c71-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="72c71-112">Methods</span></span>
|<span data-ttu-id="72c71-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="72c71-113">Method</span></span>|<span data-ttu-id="72c71-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="72c71-114">Return Type</span></span>|<span data-ttu-id="72c71-115">説明</span><span class="sxs-lookup"><span data-stu-id="72c71-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="72c71-116">deviceCategories のリスト</span><span class="sxs-lookup"><span data-stu-id="72c71-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="72c71-117">[deviceCategory](../resources/intune-shared-devicecategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="72c71-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="72c71-118">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="72c71-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="72c71-119">deviceCategory の取得</span><span class="sxs-lookup"><span data-stu-id="72c71-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="72c71-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="72c71-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="72c71-121">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="72c71-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="72c71-122">deviceCategory の作成</span><span class="sxs-lookup"><span data-stu-id="72c71-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="72c71-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="72c71-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="72c71-124">新しい [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="72c71-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="72c71-125">deviceCategory の削除</span><span class="sxs-lookup"><span data-stu-id="72c71-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="72c71-126">なし</span><span class="sxs-lookup"><span data-stu-id="72c71-126">None</span></span>|<span data-ttu-id="72c71-127">[deviceCategory](../resources/intune-shared-devicecategory.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="72c71-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="72c71-128">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="72c71-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="72c71-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="72c71-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="72c71-130">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="72c71-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="72c71-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72c71-131">Properties</span></span>
|<span data-ttu-id="72c71-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72c71-132">Property</span></span>|<span data-ttu-id="72c71-133">型</span><span class="sxs-lookup"><span data-stu-id="72c71-133">Type</span></span>|<span data-ttu-id="72c71-134">説明</span><span class="sxs-lookup"><span data-stu-id="72c71-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72c71-135">id</span><span class="sxs-lookup"><span data-stu-id="72c71-135">id</span></span>|<span data-ttu-id="72c71-136">String</span><span class="sxs-lookup"><span data-stu-id="72c71-136">String</span></span>|<span data-ttu-id="72c71-137">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="72c71-137">Unique identifier for the device category.</span></span> <span data-ttu-id="72c71-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="72c71-138">Read-only.</span></span>|
|<span data-ttu-id="72c71-139">**契約時**</span><span class="sxs-lookup"><span data-stu-id="72c71-139">**Onboarding**</span></span>|
|<span data-ttu-id="72c71-140">displayName</span><span class="sxs-lookup"><span data-stu-id="72c71-140">displayName</span></span>|<span data-ttu-id="72c71-141">String</span><span class="sxs-lookup"><span data-stu-id="72c71-141">String</span></span>|<span data-ttu-id="72c71-142">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="72c71-142">Display name for the device category.</span></span>|
|<span data-ttu-id="72c71-143">説明</span><span class="sxs-lookup"><span data-stu-id="72c71-143">description</span></span>|<span data-ttu-id="72c71-144">String</span><span class="sxs-lookup"><span data-stu-id="72c71-144">String</span></span>|<span data-ttu-id="72c71-145">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="72c71-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72c71-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="72c71-146">Relationships</span></span>
<span data-ttu-id="72c71-147">なし</span><span class="sxs-lookup"><span data-stu-id="72c71-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72c71-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="72c71-148">JSON Representation</span></span>
<span data-ttu-id="72c71-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="72c71-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



