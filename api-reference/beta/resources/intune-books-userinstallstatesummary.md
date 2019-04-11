---
title: userInstallStateSummary リソースの種類
description: ユーザーのインストール状態の要約のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ee8d92b9a9d36ddda087a20edbb8235d18811b6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774009"
---
# <a name="userinstallstatesummary-resource-type"></a><span data-ttu-id="86672-103">userInstallStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86672-103">userInstallStateSummary resource type</span></span>

> <span data-ttu-id="86672-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86672-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86672-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="86672-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86672-106">ユーザーのインストール状態の要約のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="86672-106">Contains properties for the installation state summary for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="86672-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="86672-107">Methods</span></span>
|<span data-ttu-id="86672-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="86672-108">Method</span></span>|<span data-ttu-id="86672-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="86672-109">Return Type</span></span>|<span data-ttu-id="86672-110">説明</span><span class="sxs-lookup"><span data-stu-id="86672-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="86672-111">userInstallStateSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="86672-111">List userInstallStateSummaries</span></span>](../api/intune-books-userinstallstatesummary-list.md)|<span data-ttu-id="86672-112">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="86672-112">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="86672-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="86672-113">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="86672-114">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="86672-114">Get userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-get.md)|[<span data-ttu-id="86672-115">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="86672-115">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="86672-116">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="86672-116">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="86672-117">userInstallStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="86672-117">Create userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-create.md)|[<span data-ttu-id="86672-118">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="86672-118">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="86672-119">新しい [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="86672-119">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="86672-120">userInstallStateSummary の削除</span><span class="sxs-lookup"><span data-stu-id="86672-120">Delete userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-delete.md)|<span data-ttu-id="86672-121">なし</span><span class="sxs-lookup"><span data-stu-id="86672-121">None</span></span>|<span data-ttu-id="86672-122">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="86672-122">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>|
|[<span data-ttu-id="86672-123">userInstallStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="86672-123">Update userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-update.md)|[<span data-ttu-id="86672-124">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="86672-124">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="86672-125">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="86672-125">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="86672-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86672-126">Properties</span></span>
|<span data-ttu-id="86672-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86672-127">Property</span></span>|<span data-ttu-id="86672-128">型</span><span class="sxs-lookup"><span data-stu-id="86672-128">Type</span></span>|<span data-ttu-id="86672-129">説明</span><span class="sxs-lookup"><span data-stu-id="86672-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86672-130">id</span><span class="sxs-lookup"><span data-stu-id="86672-130">id</span></span>|<span data-ttu-id="86672-131">String</span><span class="sxs-lookup"><span data-stu-id="86672-131">String</span></span>|<span data-ttu-id="86672-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="86672-132">Key of the entity.</span></span>|
|<span data-ttu-id="86672-133">userName</span><span class="sxs-lookup"><span data-stu-id="86672-133">userName</span></span>|<span data-ttu-id="86672-134">String</span><span class="sxs-lookup"><span data-stu-id="86672-134">String</span></span>|<span data-ttu-id="86672-135">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="86672-135">User name.</span></span>|
|<span data-ttu-id="86672-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86672-136">installedDeviceCount</span></span>|<span data-ttu-id="86672-137">Int32</span><span class="sxs-lookup"><span data-stu-id="86672-137">Int32</span></span>|<span data-ttu-id="86672-138">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="86672-138">Installed Device Count.</span></span>|
|<span data-ttu-id="86672-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86672-139">failedDeviceCount</span></span>|<span data-ttu-id="86672-140">Int32</span><span class="sxs-lookup"><span data-stu-id="86672-140">Int32</span></span>|<span data-ttu-id="86672-141">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="86672-141">Failed Device Count.</span></span>|
|<span data-ttu-id="86672-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86672-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="86672-143">Int32</span><span class="sxs-lookup"><span data-stu-id="86672-143">Int32</span></span>|<span data-ttu-id="86672-144">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="86672-144">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86672-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="86672-145">Relationships</span></span>
|<span data-ttu-id="86672-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="86672-146">Relationship</span></span>|<span data-ttu-id="86672-147">型</span><span class="sxs-lookup"><span data-stu-id="86672-147">Type</span></span>|<span data-ttu-id="86672-148">説明</span><span class="sxs-lookup"><span data-stu-id="86672-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86672-149">deviceStates</span><span class="sxs-lookup"><span data-stu-id="86672-149">deviceStates</span></span>|<span data-ttu-id="86672-150">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="86672-150">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="86672-151">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="86672-151">The install state of the eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86672-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86672-152">JSON Representation</span></span>
<span data-ttu-id="86672-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="86672-153">Here is a JSON representation of the resource.</span></span>
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





