---
title: userInstallStateSummary リソースの種類
description: ユーザーのインストール状態の要約のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ee8d92b9a9d36ddda087a20edbb8235d18811b6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548265"
---
# <a name="userinstallstatesummary-resource-type"></a><span data-ttu-id="42ac3-103">userInstallStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="42ac3-103">userInstallStateSummary resource type</span></span>

> <span data-ttu-id="42ac3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42ac3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42ac3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="42ac3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42ac3-106">ユーザーのインストール状態の要約のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="42ac3-106">Contains properties for the installation state summary for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="42ac3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="42ac3-107">Methods</span></span>
|<span data-ttu-id="42ac3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="42ac3-108">Method</span></span>|<span data-ttu-id="42ac3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="42ac3-109">Return Type</span></span>|<span data-ttu-id="42ac3-110">説明</span><span class="sxs-lookup"><span data-stu-id="42ac3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="42ac3-111">userInstallStateSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="42ac3-111">List userInstallStateSummaries</span></span>](../api/intune-books-userinstallstatesummary-list.md)|<span data-ttu-id="42ac3-112">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="42ac3-112">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="42ac3-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="42ac3-113">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="42ac3-114">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="42ac3-114">Get userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-get.md)|[<span data-ttu-id="42ac3-115">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="42ac3-115">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="42ac3-116">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="42ac3-116">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="42ac3-117">userInstallStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="42ac3-117">Create userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-create.md)|[<span data-ttu-id="42ac3-118">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="42ac3-118">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="42ac3-119">新しい [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="42ac3-119">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="42ac3-120">userInstallStateSummary の削除</span><span class="sxs-lookup"><span data-stu-id="42ac3-120">Delete userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-delete.md)|<span data-ttu-id="42ac3-121">なし</span><span class="sxs-lookup"><span data-stu-id="42ac3-121">None</span></span>|<span data-ttu-id="42ac3-122">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="42ac3-122">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>|
|[<span data-ttu-id="42ac3-123">userInstallStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="42ac3-123">Update userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-update.md)|[<span data-ttu-id="42ac3-124">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="42ac3-124">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="42ac3-125">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="42ac3-125">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="42ac3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42ac3-126">Properties</span></span>
|<span data-ttu-id="42ac3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42ac3-127">Property</span></span>|<span data-ttu-id="42ac3-128">型</span><span class="sxs-lookup"><span data-stu-id="42ac3-128">Type</span></span>|<span data-ttu-id="42ac3-129">説明</span><span class="sxs-lookup"><span data-stu-id="42ac3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42ac3-130">id</span><span class="sxs-lookup"><span data-stu-id="42ac3-130">id</span></span>|<span data-ttu-id="42ac3-131">String</span><span class="sxs-lookup"><span data-stu-id="42ac3-131">String</span></span>|<span data-ttu-id="42ac3-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="42ac3-132">Key of the entity.</span></span>|
|<span data-ttu-id="42ac3-133">userName</span><span class="sxs-lookup"><span data-stu-id="42ac3-133">userName</span></span>|<span data-ttu-id="42ac3-134">String</span><span class="sxs-lookup"><span data-stu-id="42ac3-134">String</span></span>|<span data-ttu-id="42ac3-135">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="42ac3-135">User name.</span></span>|
|<span data-ttu-id="42ac3-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="42ac3-136">installedDeviceCount</span></span>|<span data-ttu-id="42ac3-137">Int32</span><span class="sxs-lookup"><span data-stu-id="42ac3-137">Int32</span></span>|<span data-ttu-id="42ac3-138">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="42ac3-138">Installed Device Count.</span></span>|
|<span data-ttu-id="42ac3-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="42ac3-139">failedDeviceCount</span></span>|<span data-ttu-id="42ac3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="42ac3-140">Int32</span></span>|<span data-ttu-id="42ac3-141">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="42ac3-141">Failed Device Count.</span></span>|
|<span data-ttu-id="42ac3-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="42ac3-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="42ac3-143">Int32</span><span class="sxs-lookup"><span data-stu-id="42ac3-143">Int32</span></span>|<span data-ttu-id="42ac3-144">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="42ac3-144">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42ac3-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="42ac3-145">Relationships</span></span>
|<span data-ttu-id="42ac3-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="42ac3-146">Relationship</span></span>|<span data-ttu-id="42ac3-147">型</span><span class="sxs-lookup"><span data-stu-id="42ac3-147">Type</span></span>|<span data-ttu-id="42ac3-148">説明</span><span class="sxs-lookup"><span data-stu-id="42ac3-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42ac3-149">deviceStates</span><span class="sxs-lookup"><span data-stu-id="42ac3-149">deviceStates</span></span>|<span data-ttu-id="42ac3-150">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="42ac3-150">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="42ac3-151">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="42ac3-151">The install state of the eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42ac3-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42ac3-152">JSON Representation</span></span>
<span data-ttu-id="42ac3-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="42ac3-153">Here is a JSON representation of the resource.</span></span>
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





