---
title: deviceCategory リソースの種類
description: これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。 レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b61927b5d4c6e8c85ba454d241a0d61a20185579
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888823"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="557ff-104">deviceCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="557ff-104">deviceCategory resource type</span></span>

> <span data-ttu-id="557ff-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="557ff-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="557ff-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="557ff-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="557ff-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="557ff-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="557ff-108">カテゴリのデバイスは、デバイスを分類する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="557ff-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="557ff-109">カテゴリのデバイスを使用すると、会社の管理者は、会社に意味のある一意のカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="557ff-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="557ff-110">これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="557ff-110"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="557ff-111">レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="557ff-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="557ff-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="557ff-112">Methods</span></span>
|<span data-ttu-id="557ff-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="557ff-113">Method</span></span>|<span data-ttu-id="557ff-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="557ff-114">Return Type</span></span>|<span data-ttu-id="557ff-115">説明</span><span class="sxs-lookup"><span data-stu-id="557ff-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="557ff-116">deviceCategories のリスト</span><span class="sxs-lookup"><span data-stu-id="557ff-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="557ff-117">[deviceCategory](../resources/intune-shared-devicecategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="557ff-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="557ff-118">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="557ff-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="557ff-119">deviceCategory の取得</span><span class="sxs-lookup"><span data-stu-id="557ff-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="557ff-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="557ff-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="557ff-121">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="557ff-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="557ff-122">deviceCategory の作成</span><span class="sxs-lookup"><span data-stu-id="557ff-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="557ff-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="557ff-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="557ff-124">新しい [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="557ff-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="557ff-125">deviceCategory の削除</span><span class="sxs-lookup"><span data-stu-id="557ff-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="557ff-126">なし</span><span class="sxs-lookup"><span data-stu-id="557ff-126">None</span></span>|<span data-ttu-id="557ff-127">[deviceCategory](../resources/intune-shared-devicecategory.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="557ff-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="557ff-128">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="557ff-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="557ff-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="557ff-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="557ff-130">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="557ff-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="557ff-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="557ff-131">Properties</span></span>
|<span data-ttu-id="557ff-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="557ff-132">Property</span></span>|<span data-ttu-id="557ff-133">種類</span><span class="sxs-lookup"><span data-stu-id="557ff-133">Type</span></span>|<span data-ttu-id="557ff-134">説明</span><span class="sxs-lookup"><span data-stu-id="557ff-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="557ff-135">ID</span><span class="sxs-lookup"><span data-stu-id="557ff-135">id</span></span>|<span data-ttu-id="557ff-136">String</span><span class="sxs-lookup"><span data-stu-id="557ff-136">String</span></span>|<span data-ttu-id="557ff-137">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="557ff-137">Unique identifier for the device category.</span></span> <span data-ttu-id="557ff-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="557ff-138">Read-only.</span></span>|
|<span data-ttu-id="557ff-139">**契約時**</span><span class="sxs-lookup"><span data-stu-id="557ff-139">**Onboarding**</span></span>|
|<span data-ttu-id="557ff-140">displayName</span><span class="sxs-lookup"><span data-stu-id="557ff-140">displayName</span></span>|<span data-ttu-id="557ff-141">String</span><span class="sxs-lookup"><span data-stu-id="557ff-141">String</span></span>|<span data-ttu-id="557ff-142">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="557ff-142">Display name for the device category.</span></span>|
|<span data-ttu-id="557ff-143">説明</span><span class="sxs-lookup"><span data-stu-id="557ff-143">description</span></span>|<span data-ttu-id="557ff-144">String</span><span class="sxs-lookup"><span data-stu-id="557ff-144">String</span></span>|<span data-ttu-id="557ff-145">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="557ff-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="557ff-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="557ff-146">Relationships</span></span>
<span data-ttu-id="557ff-147">なし</span><span class="sxs-lookup"><span data-stu-id="557ff-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="557ff-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="557ff-148">JSON Representation</span></span>
<span data-ttu-id="557ff-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="557ff-149">Here is a JSON representation of the resource.</span></span>
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



