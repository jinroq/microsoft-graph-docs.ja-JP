---
title: userappinstallstatus リソースの種類
description: ユーザーのインストール状態のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3efd555f4b4a728e9a4ae660eac9568cb7e3b2a9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791118"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="e0615-103">userappinstallstatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e0615-103">userAppInstallStatus resource type</span></span>

> <span data-ttu-id="e0615-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0615-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0615-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0615-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0615-106">ユーザーのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e0615-106">Contains properties for the installation status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="e0615-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e0615-107">Methods</span></span>
|<span data-ttu-id="e0615-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e0615-108">Method</span></span>|<span data-ttu-id="e0615-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e0615-109">Return Type</span></span>|<span data-ttu-id="e0615-110">説明</span><span class="sxs-lookup"><span data-stu-id="e0615-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e0615-111">userappinstallstatuses 状態を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e0615-111">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="e0615-112">[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e0615-112">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="e0615-113">[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e0615-113">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="e0615-114">userappinstallstatus の取得</span><span class="sxs-lookup"><span data-stu-id="e0615-114">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="e0615-115">userappinstallstatus</span><span class="sxs-lookup"><span data-stu-id="e0615-115">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="e0615-116">[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e0615-116">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="e0615-117">userappinstallstatus の作成</span><span class="sxs-lookup"><span data-stu-id="e0615-117">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="e0615-118">userappinstallstatus</span><span class="sxs-lookup"><span data-stu-id="e0615-118">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="e0615-119">新しい[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e0615-119">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="e0615-120">userappinstallstatus の削除</span><span class="sxs-lookup"><span data-stu-id="e0615-120">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="e0615-121">なし</span><span class="sxs-lookup"><span data-stu-id="e0615-121">None</span></span>|<span data-ttu-id="e0615-122">[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="e0615-122">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="e0615-123">userappinstallstatus の更新</span><span class="sxs-lookup"><span data-stu-id="e0615-123">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="e0615-124">userappinstallstatus</span><span class="sxs-lookup"><span data-stu-id="e0615-124">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="e0615-125">[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e0615-125">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e0615-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0615-126">Properties</span></span>
|<span data-ttu-id="e0615-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0615-127">Property</span></span>|<span data-ttu-id="e0615-128">型</span><span class="sxs-lookup"><span data-stu-id="e0615-128">Type</span></span>|<span data-ttu-id="e0615-129">説明</span><span class="sxs-lookup"><span data-stu-id="e0615-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0615-130">id</span><span class="sxs-lookup"><span data-stu-id="e0615-130">id</span></span>|<span data-ttu-id="e0615-131">String</span><span class="sxs-lookup"><span data-stu-id="e0615-131">String</span></span>|<span data-ttu-id="e0615-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e0615-132">Key of the entity.</span></span>|
|<span data-ttu-id="e0615-133">userName</span><span class="sxs-lookup"><span data-stu-id="e0615-133">userName</span></span>|<span data-ttu-id="e0615-134">String</span><span class="sxs-lookup"><span data-stu-id="e0615-134">String</span></span>|<span data-ttu-id="e0615-135">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="e0615-135">User name.</span></span>|
|<span data-ttu-id="e0615-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e0615-136">userPrincipalName</span></span>|<span data-ttu-id="e0615-137">String</span><span class="sxs-lookup"><span data-stu-id="e0615-137">String</span></span>|<span data-ttu-id="e0615-138">ユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="e0615-138">User Principal Name.</span></span>|
|<span data-ttu-id="e0615-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0615-139">installedDeviceCount</span></span>|<span data-ttu-id="e0615-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e0615-140">Int32</span></span>|<span data-ttu-id="e0615-141">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="e0615-141">Installed Device Count.</span></span>|
|<span data-ttu-id="e0615-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0615-142">failedDeviceCount</span></span>|<span data-ttu-id="e0615-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e0615-143">Int32</span></span>|<span data-ttu-id="e0615-144">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="e0615-144">Failed Device Count.</span></span>|
|<span data-ttu-id="e0615-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0615-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="e0615-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e0615-146">Int32</span></span>|<span data-ttu-id="e0615-147">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="e0615-147">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0615-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e0615-148">Relationships</span></span>
|<span data-ttu-id="e0615-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e0615-149">Relationship</span></span>|<span data-ttu-id="e0615-150">型</span><span class="sxs-lookup"><span data-stu-id="e0615-150">Type</span></span>|<span data-ttu-id="e0615-151">説明</span><span class="sxs-lookup"><span data-stu-id="e0615-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0615-152">アプリ</span><span class="sxs-lookup"><span data-stu-id="e0615-152">app</span></span>|[<span data-ttu-id="e0615-153">mobileApp</span><span class="sxs-lookup"><span data-stu-id="e0615-153">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="e0615-154">モバイルアプリへのナビゲーションリンク。</span><span class="sxs-lookup"><span data-stu-id="e0615-154">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="e0615-155">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="e0615-155">deviceStatuses</span></span>|<span data-ttu-id="e0615-156">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e0615-156">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="e0615-157">デバイス上のアプリのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="e0615-157">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0615-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e0615-158">JSON Representation</span></span>
<span data-ttu-id="e0615-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e0615-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "String (identifier)",
  "userName": "String",
  "userPrincipalName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```





