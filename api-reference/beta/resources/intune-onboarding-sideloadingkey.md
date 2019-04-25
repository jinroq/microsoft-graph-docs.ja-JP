---
title: sideLoadingKey リソースの種類
description: SideLoadingKey エンティティは、テナントの基幹業務アプリを intall するために Windows 8 および8.1 デバイスに必要です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 698d021e6038694442e5b3a6f4b3eff2a50e9943
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566459"
---
# <a name="sideloadingkey-resource-type"></a><span data-ttu-id="96958-103">sideLoadingKey リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96958-103">sideLoadingKey resource type</span></span>

> <span data-ttu-id="96958-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96958-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96958-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="96958-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96958-106">SideLoadingKey エンティティは、テナントの基幹業務アプリを intall するために Windows 8 および8.1 デバイスに必要です。</span><span class="sxs-lookup"><span data-stu-id="96958-106">SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="96958-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="96958-107">Methods</span></span>
|<span data-ttu-id="96958-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="96958-108">Method</span></span>|<span data-ttu-id="96958-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="96958-109">Return Type</span></span>|<span data-ttu-id="96958-110">説明</span><span class="sxs-lookup"><span data-stu-id="96958-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="96958-111">リスト sideloadingkeies</span><span class="sxs-lookup"><span data-stu-id="96958-111">List sideLoadingKeies</span></span>](../api/intune-onboarding-sideloadingkey-list.md)|<span data-ttu-id="96958-112">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="96958-112">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) collection</span></span>|<span data-ttu-id="96958-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="96958-113">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>|
|[<span data-ttu-id="96958-114">sideLoadingKey を取得する</span><span class="sxs-lookup"><span data-stu-id="96958-114">Get sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-get.md)|[<span data-ttu-id="96958-115">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="96958-115">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="96958-116">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="96958-116">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="96958-117">sideLoadingKey を作成する</span><span class="sxs-lookup"><span data-stu-id="96958-117">Create sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-create.md)|[<span data-ttu-id="96958-118">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="96958-118">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="96958-119">新しい[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="96958-119">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="96958-120">sideLoadingKey の削除</span><span class="sxs-lookup"><span data-stu-id="96958-120">Delete sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-delete.md)|<span data-ttu-id="96958-121">なし</span><span class="sxs-lookup"><span data-stu-id="96958-121">None</span></span>|<span data-ttu-id="96958-122">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="96958-122">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>|
|[<span data-ttu-id="96958-123">sideLoadingKey の更新</span><span class="sxs-lookup"><span data-stu-id="96958-123">Update sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-update.md)|[<span data-ttu-id="96958-124">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="96958-124">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="96958-125">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="96958-125">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="96958-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96958-126">Properties</span></span>
|<span data-ttu-id="96958-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96958-127">Property</span></span>|<span data-ttu-id="96958-128">型</span><span class="sxs-lookup"><span data-stu-id="96958-128">Type</span></span>|<span data-ttu-id="96958-129">説明</span><span class="sxs-lookup"><span data-stu-id="96958-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96958-130">id</span><span class="sxs-lookup"><span data-stu-id="96958-130">id</span></span>|<span data-ttu-id="96958-131">String</span><span class="sxs-lookup"><span data-stu-id="96958-131">String</span></span>|<span data-ttu-id="96958-132">サイドローディングキーの一意 Id。</span><span class="sxs-lookup"><span data-stu-id="96958-132">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="96958-133">value</span><span class="sxs-lookup"><span data-stu-id="96958-133">value</span></span>|<span data-ttu-id="96958-134">文字列</span><span class="sxs-lookup"><span data-stu-id="96958-134">String</span></span>|<span data-ttu-id="96958-135">サイドローディングキー値は、5 x 5 の値で、hiphens で区切られています。</span><span class="sxs-lookup"><span data-stu-id="96958-135">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="96958-136">displayName</span><span class="sxs-lookup"><span data-stu-id="96958-136">displayName</span></span>|<span data-ttu-id="96958-137">String</span><span class="sxs-lookup"><span data-stu-id="96958-137">String</span></span>|<span data-ttu-id="96958-138">ITPro 管理者に表示されるサイドローディングキー名。</span><span class="sxs-lookup"><span data-stu-id="96958-138">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="96958-139">説明</span><span class="sxs-lookup"><span data-stu-id="96958-139">description</span></span>|<span data-ttu-id="96958-140">String</span><span class="sxs-lookup"><span data-stu-id="96958-140">String</span></span>|<span data-ttu-id="96958-141">ITPro 管理者に表示されるサイドローディングキーの説明。</span><span class="sxs-lookup"><span data-stu-id="96958-141">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="96958-142">totalactivation</span><span class="sxs-lookup"><span data-stu-id="96958-142">totalActivation</span></span>|<span data-ttu-id="96958-143">Int32</span><span class="sxs-lookup"><span data-stu-id="96958-143">Int32</span></span>|<span data-ttu-id="96958-144">ITPro 管理者に表示されるサイドローディングキーの合計です。</span><span class="sxs-lookup"><span data-stu-id="96958-144">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="96958-145">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="96958-145">lastUpdatedDateTime</span></span>|<span data-ttu-id="96958-146">String</span><span class="sxs-lookup"><span data-stu-id="96958-146">String</span></span>|<span data-ttu-id="96958-147">サイドローディングキー最終更新日が ITPro の管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="96958-147">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96958-148">関係</span><span class="sxs-lookup"><span data-stu-id="96958-148">Relationships</span></span>
<span data-ttu-id="96958-149">なし</span><span class="sxs-lookup"><span data-stu-id="96958-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96958-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96958-150">JSON Representation</span></span>
<span data-ttu-id="96958-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="96958-151">Here is a JSON representation of the resource.</span></span>
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





