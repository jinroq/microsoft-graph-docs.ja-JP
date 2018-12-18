---
title: deviceCategory リソースの種類
description: これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。 レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。
author: tfitzmac
ms.openlocfilehash: 9e40f656a7ce4d511cdb4c597c2419e8cf886c12
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353614"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="0b35d-104">deviceCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0b35d-104">deviceCategory resource type</span></span>

> <span data-ttu-id="0b35d-105">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0b35d-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b35d-106">デバイス カテゴリは、デバイスを整理する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="0b35d-106">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="0b35d-107">デバイス カテゴリを使用して、会社の管理者は、自社にとって意味のある、独自のカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="0b35d-107">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="0b35d-108">これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="0b35d-108"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="0b35d-109">レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="0b35d-109">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="0b35d-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="0b35d-110">Methods</span></span>
|<span data-ttu-id="0b35d-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="0b35d-111">Method</span></span>|<span data-ttu-id="0b35d-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0b35d-112">Return Type</span></span>|<span data-ttu-id="0b35d-113">説明</span><span class="sxs-lookup"><span data-stu-id="0b35d-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b35d-114">[リストの deviceCategories](../api/intune-shared-devicecategory-list.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0b35d-114">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="0b35d-115">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0b35d-115">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="0b35d-116">deviceCategory の取得</span><span class="sxs-lookup"><span data-stu-id="0b35d-116">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="0b35d-117">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0b35d-117">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="0b35d-118">deviceCategory の作成</span><span class="sxs-lookup"><span data-stu-id="0b35d-118">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="0b35d-119">新しい [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0b35d-119">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="0b35d-120">[DeviceCategory を削除](../api/intune-shared-devicecategory-delete.md)します。</span><span class="sxs-lookup"><span data-stu-id="0b35d-120">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="0b35d-121">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="0b35d-121">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="0b35d-122">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0b35d-122">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b35d-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b35d-123">Properties</span></span>
|<span data-ttu-id="0b35d-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b35d-124">Property</span></span>|<span data-ttu-id="0b35d-125">種類</span><span class="sxs-lookup"><span data-stu-id="0b35d-125">Type</span></span>|<span data-ttu-id="0b35d-126">説明</span><span class="sxs-lookup"><span data-stu-id="0b35d-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b35d-127">ID</span><span class="sxs-lookup"><span data-stu-id="0b35d-127">id</span></span>|<span data-ttu-id="0b35d-128">String</span><span class="sxs-lookup"><span data-stu-id="0b35d-128">String</span></span>|<span data-ttu-id="0b35d-129">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0b35d-129">Unique identifier for the device category.</span></span> <span data-ttu-id="0b35d-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0b35d-130">Read-only.</span></span>|
|<span data-ttu-id="0b35d-131">**契約時**</span><span class="sxs-lookup"><span data-stu-id="0b35d-131">**Onboarding**</span></span>|
|<span data-ttu-id="0b35d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0b35d-132">displayName</span></span>|<span data-ttu-id="0b35d-133">String</span><span class="sxs-lookup"><span data-stu-id="0b35d-133">String</span></span>|<span data-ttu-id="0b35d-134">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="0b35d-134">Display name for the device category.</span></span>|
|<span data-ttu-id="0b35d-135">説明</span><span class="sxs-lookup"><span data-stu-id="0b35d-135">description</span></span>|<span data-ttu-id="0b35d-136">String</span><span class="sxs-lookup"><span data-stu-id="0b35d-136">String</span></span>|<span data-ttu-id="0b35d-137">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="0b35d-137">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b35d-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0b35d-138">Relationships</span></span>
<span data-ttu-id="0b35d-139">なし</span><span class="sxs-lookup"><span data-stu-id="0b35d-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b35d-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0b35d-140">JSON Representation</span></span>
<span data-ttu-id="0b35d-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0b35d-141">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



