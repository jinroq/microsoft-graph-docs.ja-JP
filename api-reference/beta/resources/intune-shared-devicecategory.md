---
title: deviceCategory リソースの種類
description: これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。 レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b7470f6cf0193474bfaff4f7444ed3df1d9453a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418863"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="49cd8-104">deviceCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="49cd8-104">deviceCategory resource type</span></span>

> <span data-ttu-id="49cd8-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="49cd8-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="49cd8-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49cd8-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49cd8-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="49cd8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49cd8-108">カテゴリのデバイスは、デバイスを分類する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="49cd8-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="49cd8-109">カテゴリのデバイスを使用すると、会社の管理者は、会社に意味のある一意のカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="49cd8-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="49cd8-110">これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="49cd8-110"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="49cd8-111">レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="49cd8-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="49cd8-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="49cd8-112">Methods</span></span>
|<span data-ttu-id="49cd8-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="49cd8-113">Method</span></span>|<span data-ttu-id="49cd8-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="49cd8-114">Return Type</span></span>|<span data-ttu-id="49cd8-115">説明</span><span class="sxs-lookup"><span data-stu-id="49cd8-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="49cd8-116">deviceCategories のリスト</span><span class="sxs-lookup"><span data-stu-id="49cd8-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="49cd8-117">[deviceCategory](../resources/intune-shared-devicecategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="49cd8-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="49cd8-118">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="49cd8-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="49cd8-119">deviceCategory の取得</span><span class="sxs-lookup"><span data-stu-id="49cd8-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="49cd8-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="49cd8-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="49cd8-121">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="49cd8-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="49cd8-122">deviceCategory の作成</span><span class="sxs-lookup"><span data-stu-id="49cd8-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="49cd8-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="49cd8-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="49cd8-124">新しい [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="49cd8-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="49cd8-125">deviceCategory の削除</span><span class="sxs-lookup"><span data-stu-id="49cd8-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="49cd8-126">なし</span><span class="sxs-lookup"><span data-stu-id="49cd8-126">None</span></span>|<span data-ttu-id="49cd8-127">[deviceCategory](../resources/intune-shared-devicecategory.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="49cd8-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="49cd8-128">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="49cd8-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="49cd8-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="49cd8-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="49cd8-130">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="49cd8-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="49cd8-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49cd8-131">Properties</span></span>
|<span data-ttu-id="49cd8-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49cd8-132">Property</span></span>|<span data-ttu-id="49cd8-133">型</span><span class="sxs-lookup"><span data-stu-id="49cd8-133">Type</span></span>|<span data-ttu-id="49cd8-134">説明</span><span class="sxs-lookup"><span data-stu-id="49cd8-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49cd8-135">id</span><span class="sxs-lookup"><span data-stu-id="49cd8-135">id</span></span>|<span data-ttu-id="49cd8-136">String</span><span class="sxs-lookup"><span data-stu-id="49cd8-136">String</span></span>|<span data-ttu-id="49cd8-137">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="49cd8-137">Unique identifier for the device category.</span></span> <span data-ttu-id="49cd8-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="49cd8-138">Read-only.</span></span>|
|<span data-ttu-id="49cd8-139">**契約時**</span><span class="sxs-lookup"><span data-stu-id="49cd8-139">**Onboarding**</span></span>|
|<span data-ttu-id="49cd8-140">displayName</span><span class="sxs-lookup"><span data-stu-id="49cd8-140">displayName</span></span>|<span data-ttu-id="49cd8-141">String</span><span class="sxs-lookup"><span data-stu-id="49cd8-141">String</span></span>|<span data-ttu-id="49cd8-142">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="49cd8-142">Display name for the device category.</span></span>|
|<span data-ttu-id="49cd8-143">説明</span><span class="sxs-lookup"><span data-stu-id="49cd8-143">description</span></span>|<span data-ttu-id="49cd8-144">String</span><span class="sxs-lookup"><span data-stu-id="49cd8-144">String</span></span>|<span data-ttu-id="49cd8-145">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="49cd8-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49cd8-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49cd8-146">Relationships</span></span>
<span data-ttu-id="49cd8-147">なし</span><span class="sxs-lookup"><span data-stu-id="49cd8-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49cd8-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="49cd8-148">JSON Representation</span></span>
<span data-ttu-id="49cd8-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="49cd8-149">Here is a JSON representation of the resource.</span></span>
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



