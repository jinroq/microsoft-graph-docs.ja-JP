---
title: sideLoadingKey リソースの種類
description: SideLoadingKey エンティティは、テナントの基幹業務アプリを intall するために Windows 8 および8.1 デバイスに必要です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c09cdc1bc620c6f6882abeeae29c7e00613254b1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940142"
---
# <a name="sideloadingkey-resource-type"></a><span data-ttu-id="c41c3-103">sideLoadingKey リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c41c3-103">sideLoadingKey resource type</span></span>

> <span data-ttu-id="c41c3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c41c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c41c3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c41c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c41c3-106">SideLoadingKey エンティティは、テナントの基幹業務アプリを intall するために Windows 8 および8.1 デバイスに必要です。</span><span class="sxs-lookup"><span data-stu-id="c41c3-106">SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="c41c3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c41c3-107">Methods</span></span>
|<span data-ttu-id="c41c3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c41c3-108">Method</span></span>|<span data-ttu-id="c41c3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c41c3-109">Return Type</span></span>|<span data-ttu-id="c41c3-110">説明</span><span class="sxs-lookup"><span data-stu-id="c41c3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c41c3-111">リスト sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="c41c3-111">List sideLoadingKeies</span></span>](../api/intune-onboarding-sideloadingkey-list.md)|<span data-ttu-id="c41c3-112">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c41c3-112">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) collection</span></span>|<span data-ttu-id="c41c3-113">[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c41c3-113">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>|
|[<span data-ttu-id="c41c3-114">SideLoadingKey を取得する</span><span class="sxs-lookup"><span data-stu-id="c41c3-114">Get sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-get.md)|[<span data-ttu-id="c41c3-115">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="c41c3-115">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="c41c3-116">[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c41c3-116">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="c41c3-117">SideLoadingKey を作成する</span><span class="sxs-lookup"><span data-stu-id="c41c3-117">Create sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-create.md)|[<span data-ttu-id="c41c3-118">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="c41c3-118">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="c41c3-119">新しい[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c41c3-119">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="c41c3-120">SideLoadingKey の削除</span><span class="sxs-lookup"><span data-stu-id="c41c3-120">Delete sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-delete.md)|<span data-ttu-id="c41c3-121">None</span><span class="sxs-lookup"><span data-stu-id="c41c3-121">None</span></span>|<span data-ttu-id="c41c3-122">[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c41c3-122">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>|
|[<span data-ttu-id="c41c3-123">SideLoadingKey の更新</span><span class="sxs-lookup"><span data-stu-id="c41c3-123">Update sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-update.md)|[<span data-ttu-id="c41c3-124">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="c41c3-124">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="c41c3-125">[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c41c3-125">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c41c3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c41c3-126">Properties</span></span>
|<span data-ttu-id="c41c3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c41c3-127">Property</span></span>|<span data-ttu-id="c41c3-128">型</span><span class="sxs-lookup"><span data-stu-id="c41c3-128">Type</span></span>|<span data-ttu-id="c41c3-129">説明</span><span class="sxs-lookup"><span data-stu-id="c41c3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c41c3-130">id</span><span class="sxs-lookup"><span data-stu-id="c41c3-130">id</span></span>|<span data-ttu-id="c41c3-131">文字列</span><span class="sxs-lookup"><span data-stu-id="c41c3-131">String</span></span>|<span data-ttu-id="c41c3-132">サイドローディングキーの一意 Id。</span><span class="sxs-lookup"><span data-stu-id="c41c3-132">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="c41c3-133">value</span><span class="sxs-lookup"><span data-stu-id="c41c3-133">value</span></span>|<span data-ttu-id="c41c3-134">文字列</span><span class="sxs-lookup"><span data-stu-id="c41c3-134">String</span></span>|<span data-ttu-id="c41c3-135">サイドローディングキー値は、5 x 5 の値で、hiphens で区切られています。</span><span class="sxs-lookup"><span data-stu-id="c41c3-135">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="c41c3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c41c3-136">displayName</span></span>|<span data-ttu-id="c41c3-137">String</span><span class="sxs-lookup"><span data-stu-id="c41c3-137">String</span></span>|<span data-ttu-id="c41c3-138">ITPro 管理者に表示されるサイドローディングキー名。</span><span class="sxs-lookup"><span data-stu-id="c41c3-138">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="c41c3-139">description</span><span class="sxs-lookup"><span data-stu-id="c41c3-139">description</span></span>|<span data-ttu-id="c41c3-140">String</span><span class="sxs-lookup"><span data-stu-id="c41c3-140">String</span></span>|<span data-ttu-id="c41c3-141">ITPro 管理者に表示されるサイドローディングキーの説明。</span><span class="sxs-lookup"><span data-stu-id="c41c3-141">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="c41c3-142">totalActivation</span><span class="sxs-lookup"><span data-stu-id="c41c3-142">totalActivation</span></span>|<span data-ttu-id="c41c3-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c41c3-143">Int32</span></span>|<span data-ttu-id="c41c3-144">ITPro 管理者に表示されるサイドローディングキーの合計です。</span><span class="sxs-lookup"><span data-stu-id="c41c3-144">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="c41c3-145">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c41c3-145">lastUpdatedDateTime</span></span>|<span data-ttu-id="c41c3-146">String</span><span class="sxs-lookup"><span data-stu-id="c41c3-146">String</span></span>|<span data-ttu-id="c41c3-147">サイドローディングキー最終更新日が ITPro の管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="c41c3-147">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c41c3-148">関係</span><span class="sxs-lookup"><span data-stu-id="c41c3-148">Relationships</span></span>
<span data-ttu-id="c41c3-149">なし</span><span class="sxs-lookup"><span data-stu-id="c41c3-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c41c3-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c41c3-150">JSON Representation</span></span>
<span data-ttu-id="c41c3-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c41c3-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sideLoadingKey"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "String (identifier)",
  "value": "String",
  "displayName": "String",
  "description": "String",
  "totalActivation": 1024,
  "lastUpdatedDateTime": "String"
}
```




