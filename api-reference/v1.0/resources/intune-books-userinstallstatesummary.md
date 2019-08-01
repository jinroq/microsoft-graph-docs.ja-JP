---
title: userInstallStateSummary リソースの種類
description: ユーザーのインストール状態の要約のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 04b551a408843e9951c2ba2626551464d8e356f6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028785"
---
# <a name="userinstallstatesummary-resource-type"></a><span data-ttu-id="6bc5e-103">userInstallStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6bc5e-103">userInstallStateSummary resource type</span></span>

> <span data-ttu-id="6bc5e-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6bc5e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bc5e-105">ユーザーのインストール状態の要約のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6bc5e-105">Contains properties for the installation state summary for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="6bc5e-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="6bc5e-106">Methods</span></span>
|<span data-ttu-id="6bc5e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6bc5e-107">Method</span></span>|<span data-ttu-id="6bc5e-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6bc5e-108">Return Type</span></span>|<span data-ttu-id="6bc5e-109">説明</span><span class="sxs-lookup"><span data-stu-id="6bc5e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6bc5e-110">userInstallStateSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="6bc5e-110">List userInstallStateSummaries</span></span>](../api/intune-books-userinstallstatesummary-list.md)|<span data-ttu-id="6bc5e-111">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6bc5e-111">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="6bc5e-112">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6bc5e-112">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="6bc5e-113">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="6bc5e-113">Get userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-get.md)|[<span data-ttu-id="6bc5e-114">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="6bc5e-114">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="6bc5e-115">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6bc5e-115">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="6bc5e-116">userInstallStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="6bc5e-116">Create userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-create.md)|[<span data-ttu-id="6bc5e-117">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="6bc5e-117">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="6bc5e-118">新しい [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6bc5e-118">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="6bc5e-119">userInstallStateSummary の削除</span><span class="sxs-lookup"><span data-stu-id="6bc5e-119">Delete userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-delete.md)|<span data-ttu-id="6bc5e-120">None</span><span class="sxs-lookup"><span data-stu-id="6bc5e-120">None</span></span>|<span data-ttu-id="6bc5e-121">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6bc5e-121">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>|
|[<span data-ttu-id="6bc5e-122">userInstallStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="6bc5e-122">Update userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-update.md)|[<span data-ttu-id="6bc5e-123">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="6bc5e-123">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="6bc5e-124">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6bc5e-124">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6bc5e-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6bc5e-125">Properties</span></span>
|<span data-ttu-id="6bc5e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6bc5e-126">Property</span></span>|<span data-ttu-id="6bc5e-127">型</span><span class="sxs-lookup"><span data-stu-id="6bc5e-127">Type</span></span>|<span data-ttu-id="6bc5e-128">説明</span><span class="sxs-lookup"><span data-stu-id="6bc5e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bc5e-129">id</span><span class="sxs-lookup"><span data-stu-id="6bc5e-129">id</span></span>|<span data-ttu-id="6bc5e-130">String</span><span class="sxs-lookup"><span data-stu-id="6bc5e-130">String</span></span>|<span data-ttu-id="6bc5e-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6bc5e-131">Key of the entity.</span></span>|
|<span data-ttu-id="6bc5e-132">userName</span><span class="sxs-lookup"><span data-stu-id="6bc5e-132">userName</span></span>|<span data-ttu-id="6bc5e-133">String</span><span class="sxs-lookup"><span data-stu-id="6bc5e-133">String</span></span>|<span data-ttu-id="6bc5e-134">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="6bc5e-134">User name.</span></span>|
|<span data-ttu-id="6bc5e-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6bc5e-135">installedDeviceCount</span></span>|<span data-ttu-id="6bc5e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6bc5e-136">Int32</span></span>|<span data-ttu-id="6bc5e-137">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="6bc5e-137">Installed Device Count.</span></span>|
|<span data-ttu-id="6bc5e-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6bc5e-138">failedDeviceCount</span></span>|<span data-ttu-id="6bc5e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6bc5e-139">Int32</span></span>|<span data-ttu-id="6bc5e-140">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="6bc5e-140">Failed Device Count.</span></span>|
|<span data-ttu-id="6bc5e-141">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6bc5e-141">notInstalledDeviceCount</span></span>|<span data-ttu-id="6bc5e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6bc5e-142">Int32</span></span>|<span data-ttu-id="6bc5e-143">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="6bc5e-143">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bc5e-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6bc5e-144">Relationships</span></span>
|<span data-ttu-id="6bc5e-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6bc5e-145">Relationship</span></span>|<span data-ttu-id="6bc5e-146">型</span><span class="sxs-lookup"><span data-stu-id="6bc5e-146">Type</span></span>|<span data-ttu-id="6bc5e-147">説明</span><span class="sxs-lookup"><span data-stu-id="6bc5e-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bc5e-148">deviceStates</span><span class="sxs-lookup"><span data-stu-id="6bc5e-148">deviceStates</span></span>|<span data-ttu-id="6bc5e-149">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6bc5e-149">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="6bc5e-150">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="6bc5e-150">The install state of the eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6bc5e-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6bc5e-151">JSON Representation</span></span>
<span data-ttu-id="6bc5e-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6bc5e-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userInstallStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "String (identifier)",
  "userName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```



