---
title: userAppInstallStatus リソースの種類
description: ユーザーのインストール状態のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2f8c4b31a3c30210c1fbf9de6af5f7d00a939ea
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949704"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="ae938-103">userAppInstallStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ae938-103">userAppInstallStatus resource type</span></span>

> <span data-ttu-id="ae938-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae938-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae938-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae938-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae938-106">ユーザーのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ae938-106">Contains properties for the installation status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="ae938-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ae938-107">Methods</span></span>
|<span data-ttu-id="ae938-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ae938-108">Method</span></span>|<span data-ttu-id="ae938-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ae938-109">Return Type</span></span>|<span data-ttu-id="ae938-110">説明</span><span class="sxs-lookup"><span data-stu-id="ae938-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ae938-111">UserAppInstallStatuses 状態を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ae938-111">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="ae938-112">[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ae938-112">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="ae938-113">[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ae938-113">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="ae938-114">UserAppInstallStatus の取得</span><span class="sxs-lookup"><span data-stu-id="ae938-114">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="ae938-115">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ae938-115">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="ae938-116">[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ae938-116">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="ae938-117">UserAppInstallStatus の作成</span><span class="sxs-lookup"><span data-stu-id="ae938-117">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="ae938-118">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ae938-118">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="ae938-119">新しい[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ae938-119">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="ae938-120">UserAppInstallStatus の削除</span><span class="sxs-lookup"><span data-stu-id="ae938-120">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="ae938-121">None</span><span class="sxs-lookup"><span data-stu-id="ae938-121">None</span></span>|<span data-ttu-id="ae938-122">[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="ae938-122">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="ae938-123">UserAppInstallStatus の更新</span><span class="sxs-lookup"><span data-stu-id="ae938-123">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="ae938-124">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ae938-124">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="ae938-125">[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ae938-125">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae938-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae938-126">Properties</span></span>
|<span data-ttu-id="ae938-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae938-127">Property</span></span>|<span data-ttu-id="ae938-128">種類</span><span class="sxs-lookup"><span data-stu-id="ae938-128">Type</span></span>|<span data-ttu-id="ae938-129">説明</span><span class="sxs-lookup"><span data-stu-id="ae938-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae938-130">id</span><span class="sxs-lookup"><span data-stu-id="ae938-130">id</span></span>|<span data-ttu-id="ae938-131">文字列</span><span class="sxs-lookup"><span data-stu-id="ae938-131">String</span></span>|<span data-ttu-id="ae938-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ae938-132">Key of the entity.</span></span>|
|<span data-ttu-id="ae938-133">userName</span><span class="sxs-lookup"><span data-stu-id="ae938-133">userName</span></span>|<span data-ttu-id="ae938-134">String</span><span class="sxs-lookup"><span data-stu-id="ae938-134">String</span></span>|<span data-ttu-id="ae938-135">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="ae938-135">User name.</span></span>|
|<span data-ttu-id="ae938-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ae938-136">userPrincipalName</span></span>|<span data-ttu-id="ae938-137">String</span><span class="sxs-lookup"><span data-stu-id="ae938-137">String</span></span>|<span data-ttu-id="ae938-138">ユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="ae938-138">User Principal Name.</span></span>|
|<span data-ttu-id="ae938-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae938-139">installedDeviceCount</span></span>|<span data-ttu-id="ae938-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ae938-140">Int32</span></span>|<span data-ttu-id="ae938-141">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ae938-141">Installed Device Count.</span></span>|
|<span data-ttu-id="ae938-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae938-142">failedDeviceCount</span></span>|<span data-ttu-id="ae938-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ae938-143">Int32</span></span>|<span data-ttu-id="ae938-144">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ae938-144">Failed Device Count.</span></span>|
|<span data-ttu-id="ae938-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae938-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="ae938-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ae938-146">Int32</span></span>|<span data-ttu-id="ae938-147">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ae938-147">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae938-148">関係</span><span class="sxs-lookup"><span data-stu-id="ae938-148">Relationships</span></span>
|<span data-ttu-id="ae938-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ae938-149">Relationship</span></span>|<span data-ttu-id="ae938-150">型</span><span class="sxs-lookup"><span data-stu-id="ae938-150">Type</span></span>|<span data-ttu-id="ae938-151">説明</span><span class="sxs-lookup"><span data-stu-id="ae938-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae938-152">アプリ</span><span class="sxs-lookup"><span data-stu-id="ae938-152">app</span></span>|[<span data-ttu-id="ae938-153">mobileApp</span><span class="sxs-lookup"><span data-stu-id="ae938-153">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="ae938-154">モバイルアプリへのナビゲーションリンク。</span><span class="sxs-lookup"><span data-stu-id="ae938-154">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="ae938-155">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="ae938-155">deviceStatuses</span></span>|<span data-ttu-id="ae938-156">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ae938-156">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="ae938-157">デバイス上のアプリのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="ae938-157">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae938-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ae938-158">JSON Representation</span></span>
<span data-ttu-id="ae938-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ae938-159">Here is a JSON representation of the resource.</span></span>
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




