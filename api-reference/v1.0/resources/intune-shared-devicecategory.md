---
title: deviceCategory リソースの種類
description: これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。 レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 269b022692e04ad3f646b25c3f78045ba42a51a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036989"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="d41fc-104">deviceCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d41fc-104">deviceCategory resource type</span></span>

> <span data-ttu-id="d41fc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d41fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d41fc-106">デバイス カテゴリは、デバイスを整理する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="d41fc-106">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="d41fc-107">デバイス カテゴリを使用して、会社の管理者は、自社にとって意味のある、独自のカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="d41fc-107">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="d41fc-108">これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="d41fc-108"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="d41fc-109">レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="d41fc-109">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="d41fc-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="d41fc-110">Methods</span></span>
|<span data-ttu-id="d41fc-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="d41fc-111">Method</span></span>|<span data-ttu-id="d41fc-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d41fc-112">Return Type</span></span>|<span data-ttu-id="d41fc-113">説明</span><span class="sxs-lookup"><span data-stu-id="d41fc-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d41fc-114">[DeviceCategories コレクションを一覧表示](../api/intune-shared-devicecategory-list.md)する</span><span class="sxs-lookup"><span data-stu-id="d41fc-114">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="d41fc-115">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d41fc-115">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="d41fc-116">deviceCategory の取得</span><span class="sxs-lookup"><span data-stu-id="d41fc-116">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="d41fc-117">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d41fc-117">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="d41fc-118">deviceCategory の作成</span><span class="sxs-lookup"><span data-stu-id="d41fc-118">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="d41fc-119">新しい [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d41fc-119">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="d41fc-120">[DeviceCategory を削除](../api/intune-shared-devicecategory-delete.md)します。</span><span class="sxs-lookup"><span data-stu-id="d41fc-120">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="d41fc-121">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="d41fc-121">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="d41fc-122">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d41fc-122">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d41fc-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d41fc-123">Properties</span></span>
|<span data-ttu-id="d41fc-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d41fc-124">Property</span></span>|<span data-ttu-id="d41fc-125">型</span><span class="sxs-lookup"><span data-stu-id="d41fc-125">Type</span></span>|<span data-ttu-id="d41fc-126">説明</span><span class="sxs-lookup"><span data-stu-id="d41fc-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d41fc-127">id</span><span class="sxs-lookup"><span data-stu-id="d41fc-127">id</span></span>|<span data-ttu-id="d41fc-128">文字列</span><span class="sxs-lookup"><span data-stu-id="d41fc-128">String</span></span>|<span data-ttu-id="d41fc-129">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d41fc-129">Unique identifier for the device category.</span></span> <span data-ttu-id="d41fc-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d41fc-130">Read-only.</span></span>|
|<span data-ttu-id="d41fc-131">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="d41fc-131">**Onboarding**</span></span>|
|<span data-ttu-id="d41fc-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d41fc-132">displayName</span></span>|<span data-ttu-id="d41fc-133">String</span><span class="sxs-lookup"><span data-stu-id="d41fc-133">String</span></span>|<span data-ttu-id="d41fc-134">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="d41fc-134">Display name for the device category.</span></span>|
|<span data-ttu-id="d41fc-135">description</span><span class="sxs-lookup"><span data-stu-id="d41fc-135">description</span></span>|<span data-ttu-id="d41fc-136">String</span><span class="sxs-lookup"><span data-stu-id="d41fc-136">String</span></span>|<span data-ttu-id="d41fc-137">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="d41fc-137">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d41fc-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d41fc-138">Relationships</span></span>
<span data-ttu-id="d41fc-139">なし</span><span class="sxs-lookup"><span data-stu-id="d41fc-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d41fc-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d41fc-140">JSON Representation</span></span>
<span data-ttu-id="d41fc-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d41fc-141">Here is a JSON representation of the resource.</span></span>
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



