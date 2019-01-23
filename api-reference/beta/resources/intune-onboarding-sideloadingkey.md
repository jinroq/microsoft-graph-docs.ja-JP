---
title: sideLoadingKey リソースの種類
description: SideLoadingKey エンティティは、Windows 8 とテナントのビジネス アプリケーションのインストールの行に 8.1 のデバイスに必要です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f7be853faae78e0ac7528d0127fd11b928164ee9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410043"
---
# <a name="sideloadingkey-resource-type"></a><span data-ttu-id="bbdeb-103">sideLoadingKey リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bbdeb-103">sideLoadingKey resource type</span></span>

> <span data-ttu-id="bbdeb-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bbdeb-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bbdeb-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbdeb-107">SideLoadingKey エンティティは、Windows 8 とテナントのビジネス アプリケーションのインストールの行に 8.1 のデバイスに必要です。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-107">SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="bbdeb-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bbdeb-108">Methods</span></span>
|<span data-ttu-id="bbdeb-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="bbdeb-109">Method</span></span>|<span data-ttu-id="bbdeb-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bbdeb-110">Return Type</span></span>|<span data-ttu-id="bbdeb-111">説明</span><span class="sxs-lookup"><span data-stu-id="bbdeb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bbdeb-112">リスト sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="bbdeb-112">List sideLoadingKeies</span></span>](../api/intune-onboarding-sideloadingkey-list.md)|<span data-ttu-id="bbdeb-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bbdeb-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) collection</span></span>|<span data-ttu-id="bbdeb-114">[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-114">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>|
|[<span data-ttu-id="bbdeb-115">SideLoadingKey を取得します。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-115">Get sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-get.md)|[<span data-ttu-id="bbdeb-116">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="bbdeb-116">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="bbdeb-117">[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-117">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="bbdeb-118">SideLoadingKey を作成します。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-118">Create sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-create.md)|[<span data-ttu-id="bbdeb-119">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="bbdeb-119">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="bbdeb-120">新しい[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-120">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="bbdeb-121">SideLoadingKey を削除します。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-121">Delete sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-delete.md)|<span data-ttu-id="bbdeb-122">なし</span><span class="sxs-lookup"><span data-stu-id="bbdeb-122">None</span></span>|<span data-ttu-id="bbdeb-123">の[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-123">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>|
|[<span data-ttu-id="bbdeb-124">SideLoadingKey を更新します。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-124">Update sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-update.md)|[<span data-ttu-id="bbdeb-125">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="bbdeb-125">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="bbdeb-126">[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-126">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bbdeb-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbdeb-127">Properties</span></span>
|<span data-ttu-id="bbdeb-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbdeb-128">Property</span></span>|<span data-ttu-id="bbdeb-129">型</span><span class="sxs-lookup"><span data-stu-id="bbdeb-129">Type</span></span>|<span data-ttu-id="bbdeb-130">説明</span><span class="sxs-lookup"><span data-stu-id="bbdeb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbdeb-131">id</span><span class="sxs-lookup"><span data-stu-id="bbdeb-131">id</span></span>|<span data-ttu-id="bbdeb-132">String</span><span class="sxs-lookup"><span data-stu-id="bbdeb-132">String</span></span>|<span data-ttu-id="bbdeb-133">側のキーの一意の id の読み込み</span><span class="sxs-lookup"><span data-stu-id="bbdeb-133">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="bbdeb-134">value</span><span class="sxs-lookup"><span data-stu-id="bbdeb-134">value</span></span>|<span data-ttu-id="bbdeb-135">文字列</span><span class="sxs-lookup"><span data-stu-id="bbdeb-135">String</span></span>|<span data-ttu-id="bbdeb-136">側の読み込みキー] の値は 5 列 5 行値、hiphens によって区切られています。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-136">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="bbdeb-137">displayName</span><span class="sxs-lookup"><span data-stu-id="bbdeb-137">displayName</span></span>|<span data-ttu-id="bbdeb-138">String</span><span class="sxs-lookup"><span data-stu-id="bbdeb-138">String</span></span>|<span data-ttu-id="bbdeb-139">側の読み込みキー名、it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-139">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="bbdeb-140">説明</span><span class="sxs-lookup"><span data-stu-id="bbdeb-140">description</span></span>|<span data-ttu-id="bbdeb-141">String</span><span class="sxs-lookup"><span data-stu-id="bbdeb-141">String</span></span>|<span data-ttu-id="bbdeb-142">側キーの読み込み中の説明は、it プロフェッショナルの管理者に表示されます.</span><span class="sxs-lookup"><span data-stu-id="bbdeb-142">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="bbdeb-143">totalActivation</span><span class="sxs-lookup"><span data-stu-id="bbdeb-143">totalActivation</span></span>|<span data-ttu-id="bbdeb-144">Int32</span><span class="sxs-lookup"><span data-stu-id="bbdeb-144">Int32</span></span>|<span data-ttu-id="bbdeb-145">側の読み込みキー合計のアクティブ化、it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-145">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="bbdeb-146">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bbdeb-146">lastUpdatedDateTime</span></span>|<span data-ttu-id="bbdeb-147">String</span><span class="sxs-lookup"><span data-stu-id="bbdeb-147">String</span></span>|<span data-ttu-id="bbdeb-148">側の読み込みキー最終更新日 it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-148">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbdeb-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bbdeb-149">Relationships</span></span>
<span data-ttu-id="bbdeb-150">なし</span><span class="sxs-lookup"><span data-stu-id="bbdeb-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbdeb-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bbdeb-151">JSON Representation</span></span>
<span data-ttu-id="bbdeb-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bbdeb-152">Here is a JSON representation of the resource.</span></span>
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




