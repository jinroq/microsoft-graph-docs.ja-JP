---
title: sideLoadingKey リソースの種類
description: SideLoadingKey エンティティは、Windows 8 とテナントのビジネス アプリケーションのインストールの行に 8.1 のデバイスに必要です。
ms.openlocfilehash: cac2360e2c50e64e1b421df4efaf53802d78558b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074090"
---
# <a name="sideloadingkey-resource-type"></a><span data-ttu-id="d1880-103">sideLoadingKey リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1880-103">sideLoadingKey resource type</span></span>

> <span data-ttu-id="d1880-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d1880-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1880-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1880-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1880-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d1880-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1880-107">SideLoadingKey エンティティは、Windows 8 とテナントのビジネス アプリケーションのインストールの行に 8.1 のデバイスに必要です。</span><span class="sxs-lookup"><span data-stu-id="d1880-107">SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="d1880-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d1880-108">Methods</span></span>
|<span data-ttu-id="d1880-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d1880-109">Method</span></span>|<span data-ttu-id="d1880-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d1880-110">Return Type</span></span>|<span data-ttu-id="d1880-111">説明</span><span class="sxs-lookup"><span data-stu-id="d1880-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d1880-112">リスト sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="d1880-112">List sideLoadingKeies</span></span>](../api/intune-onboarding-sideloadingkey-list.md)|<span data-ttu-id="d1880-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d1880-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) collection</span></span>|<span data-ttu-id="d1880-114">[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d1880-114">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>|
|[<span data-ttu-id="d1880-115">SideLoadingKey を取得します。</span><span class="sxs-lookup"><span data-stu-id="d1880-115">Get sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-get.md)|[<span data-ttu-id="d1880-116">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="d1880-116">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="d1880-117">[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1880-117">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="d1880-118">SideLoadingKey を作成します。</span><span class="sxs-lookup"><span data-stu-id="d1880-118">Create sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-create.md)|[<span data-ttu-id="d1880-119">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="d1880-119">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="d1880-120">新しい[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d1880-120">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="d1880-121">SideLoadingKey を削除します。</span><span class="sxs-lookup"><span data-stu-id="d1880-121">Delete sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-delete.md)|<span data-ttu-id="d1880-122">なし</span><span class="sxs-lookup"><span data-stu-id="d1880-122">None</span></span>|<span data-ttu-id="d1880-123">の[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="d1880-123">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>|
|[<span data-ttu-id="d1880-124">SideLoadingKey を更新します。</span><span class="sxs-lookup"><span data-stu-id="d1880-124">Update sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-update.md)|[<span data-ttu-id="d1880-125">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="d1880-125">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="d1880-126">[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d1880-126">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d1880-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1880-127">Properties</span></span>
|<span data-ttu-id="d1880-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1880-128">Property</span></span>|<span data-ttu-id="d1880-129">型</span><span class="sxs-lookup"><span data-stu-id="d1880-129">Type</span></span>|<span data-ttu-id="d1880-130">説明</span><span class="sxs-lookup"><span data-stu-id="d1880-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1880-131">id</span><span class="sxs-lookup"><span data-stu-id="d1880-131">id</span></span>|<span data-ttu-id="d1880-132">String</span><span class="sxs-lookup"><span data-stu-id="d1880-132">String</span></span>|<span data-ttu-id="d1880-133">側のキーの一意の id の読み込み</span><span class="sxs-lookup"><span data-stu-id="d1880-133">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="d1880-134">value</span><span class="sxs-lookup"><span data-stu-id="d1880-134">value</span></span>|<span data-ttu-id="d1880-135">文字列</span><span class="sxs-lookup"><span data-stu-id="d1880-135">String</span></span>|<span data-ttu-id="d1880-136">側の読み込みキー] の値は 5 列 5 行値、hiphens によって区切られています。</span><span class="sxs-lookup"><span data-stu-id="d1880-136">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="d1880-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d1880-137">displayName</span></span>|<span data-ttu-id="d1880-138">String</span><span class="sxs-lookup"><span data-stu-id="d1880-138">String</span></span>|<span data-ttu-id="d1880-139">側の読み込みキー名、it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="d1880-139">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="d1880-140">説明</span><span class="sxs-lookup"><span data-stu-id="d1880-140">description</span></span>|<span data-ttu-id="d1880-141">String</span><span class="sxs-lookup"><span data-stu-id="d1880-141">String</span></span>|<span data-ttu-id="d1880-142">側キーの読み込み中の説明は、it プロフェッショナルの管理者に表示されます.</span><span class="sxs-lookup"><span data-stu-id="d1880-142">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="d1880-143">totalActivation</span><span class="sxs-lookup"><span data-stu-id="d1880-143">totalActivation</span></span>|<span data-ttu-id="d1880-144">Int32</span><span class="sxs-lookup"><span data-stu-id="d1880-144">Int32</span></span>|<span data-ttu-id="d1880-145">側の読み込みキー合計のアクティブ化、it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="d1880-145">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="d1880-146">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1880-146">lastUpdatedDateTime</span></span>|<span data-ttu-id="d1880-147">String</span><span class="sxs-lookup"><span data-stu-id="d1880-147">String</span></span>|<span data-ttu-id="d1880-148">側の読み込みキー最終更新日 it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="d1880-148">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1880-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d1880-149">Relationships</span></span>
<span data-ttu-id="d1880-150">なし</span><span class="sxs-lookup"><span data-stu-id="d1880-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d1880-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1880-151">JSON Representation</span></span>
<span data-ttu-id="d1880-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d1880-152">Here is a JSON representation of the resource.</span></span>
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





