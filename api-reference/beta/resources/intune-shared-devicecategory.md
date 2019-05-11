---
title: deviceCategory リソースの種類
description: これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。 レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ff6c9d5bccb48338d88e0698ee58c0121cf49101
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939715"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="a4729-104">deviceCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4729-104">deviceCategory resource type</span></span>

> <span data-ttu-id="a4729-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4729-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4729-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4729-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4729-107">デバイスカテゴリは、デバイスを整理する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="a4729-107">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="a4729-108">会社の管理者は、デバイスカテゴリを使用して、会社にとって意味のある一意のカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="a4729-108">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="a4729-109">これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="a4729-109"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="a4729-110">レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="a4729-110">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="a4729-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4729-111">Methods</span></span>
|<span data-ttu-id="a4729-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4729-112">Method</span></span>|<span data-ttu-id="a4729-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a4729-113">Return Type</span></span>|<span data-ttu-id="a4729-114">説明</span><span class="sxs-lookup"><span data-stu-id="a4729-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a4729-115">deviceCategories のリスト</span><span class="sxs-lookup"><span data-stu-id="a4729-115">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="a4729-116">[deviceCategory](../resources/intune-shared-devicecategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a4729-116">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="a4729-117">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a4729-117">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="a4729-118">deviceCategory の取得</span><span class="sxs-lookup"><span data-stu-id="a4729-118">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="a4729-119">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="a4729-119">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="a4729-120">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a4729-120">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="a4729-121">deviceCategory の作成</span><span class="sxs-lookup"><span data-stu-id="a4729-121">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="a4729-122">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="a4729-122">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="a4729-123">新しい [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a4729-123">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="a4729-124">deviceCategory の削除</span><span class="sxs-lookup"><span data-stu-id="a4729-124">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="a4729-125">なし</span><span class="sxs-lookup"><span data-stu-id="a4729-125">None</span></span>|<span data-ttu-id="a4729-126">[deviceCategory](../resources/intune-shared-devicecategory.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="a4729-126">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="a4729-127">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="a4729-127">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="a4729-128">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="a4729-128">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="a4729-129">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a4729-129">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a4729-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4729-130">Properties</span></span>
|<span data-ttu-id="a4729-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4729-131">Property</span></span>|<span data-ttu-id="a4729-132">型</span><span class="sxs-lookup"><span data-stu-id="a4729-132">Type</span></span>|<span data-ttu-id="a4729-133">説明</span><span class="sxs-lookup"><span data-stu-id="a4729-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4729-134">id</span><span class="sxs-lookup"><span data-stu-id="a4729-134">id</span></span>|<span data-ttu-id="a4729-135">文字列</span><span class="sxs-lookup"><span data-stu-id="a4729-135">String</span></span>|<span data-ttu-id="a4729-136">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a4729-136">Unique identifier for the device category.</span></span> <span data-ttu-id="a4729-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a4729-137">Read-only.</span></span>|
|<span data-ttu-id="a4729-138">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="a4729-138">**Onboarding**</span></span>|
|<span data-ttu-id="a4729-139">displayName</span><span class="sxs-lookup"><span data-stu-id="a4729-139">displayName</span></span>|<span data-ttu-id="a4729-140">String</span><span class="sxs-lookup"><span data-stu-id="a4729-140">String</span></span>|<span data-ttu-id="a4729-141">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="a4729-141">Display name for the device category.</span></span>|
|<span data-ttu-id="a4729-142">description</span><span class="sxs-lookup"><span data-stu-id="a4729-142">description</span></span>|<span data-ttu-id="a4729-143">String</span><span class="sxs-lookup"><span data-stu-id="a4729-143">String</span></span>|<span data-ttu-id="a4729-144">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="a4729-144">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4729-145">関係</span><span class="sxs-lookup"><span data-stu-id="a4729-145">Relationships</span></span>
<span data-ttu-id="a4729-146">なし</span><span class="sxs-lookup"><span data-stu-id="a4729-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4729-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4729-147">JSON Representation</span></span>
<span data-ttu-id="a4729-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a4729-148">Here is a JSON representation of the resource.</span></span>
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



