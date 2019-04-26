---
title: userappinstallstatus リソースの種類
description: ユーザーのインストール状態のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3efd555f4b4a728e9a4ae660eac9568cb7e3b2a9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555109"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="7a1d3-103">userappinstallstatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7a1d3-103">userAppInstallStatus resource type</span></span>

> <span data-ttu-id="7a1d3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a1d3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a1d3-106">ユーザーのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-106">Contains properties for the installation status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="7a1d3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7a1d3-107">Methods</span></span>
|<span data-ttu-id="7a1d3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7a1d3-108">Method</span></span>|<span data-ttu-id="7a1d3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7a1d3-109">Return Type</span></span>|<span data-ttu-id="7a1d3-110">説明</span><span class="sxs-lookup"><span data-stu-id="7a1d3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7a1d3-111">userappinstallstatuses 状態を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7a1d3-111">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="7a1d3-112">[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7a1d3-112">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="7a1d3-113">[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-113">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="7a1d3-114">userappinstallstatus の取得</span><span class="sxs-lookup"><span data-stu-id="7a1d3-114">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="7a1d3-115">userappinstallstatus</span><span class="sxs-lookup"><span data-stu-id="7a1d3-115">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="7a1d3-116">[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-116">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="7a1d3-117">userappinstallstatus の作成</span><span class="sxs-lookup"><span data-stu-id="7a1d3-117">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="7a1d3-118">userappinstallstatus</span><span class="sxs-lookup"><span data-stu-id="7a1d3-118">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="7a1d3-119">新しい[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-119">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="7a1d3-120">userappinstallstatus の削除</span><span class="sxs-lookup"><span data-stu-id="7a1d3-120">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="7a1d3-121">なし</span><span class="sxs-lookup"><span data-stu-id="7a1d3-121">None</span></span>|<span data-ttu-id="7a1d3-122">[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-122">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="7a1d3-123">userappinstallstatus の更新</span><span class="sxs-lookup"><span data-stu-id="7a1d3-123">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="7a1d3-124">userappinstallstatus</span><span class="sxs-lookup"><span data-stu-id="7a1d3-124">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="7a1d3-125">[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-125">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7a1d3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a1d3-126">Properties</span></span>
|<span data-ttu-id="7a1d3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a1d3-127">Property</span></span>|<span data-ttu-id="7a1d3-128">型</span><span class="sxs-lookup"><span data-stu-id="7a1d3-128">Type</span></span>|<span data-ttu-id="7a1d3-129">説明</span><span class="sxs-lookup"><span data-stu-id="7a1d3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a1d3-130">id</span><span class="sxs-lookup"><span data-stu-id="7a1d3-130">id</span></span>|<span data-ttu-id="7a1d3-131">String</span><span class="sxs-lookup"><span data-stu-id="7a1d3-131">String</span></span>|<span data-ttu-id="7a1d3-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-132">Key of the entity.</span></span>|
|<span data-ttu-id="7a1d3-133">userName</span><span class="sxs-lookup"><span data-stu-id="7a1d3-133">userName</span></span>|<span data-ttu-id="7a1d3-134">String</span><span class="sxs-lookup"><span data-stu-id="7a1d3-134">String</span></span>|<span data-ttu-id="7a1d3-135">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-135">User name.</span></span>|
|<span data-ttu-id="7a1d3-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7a1d3-136">userPrincipalName</span></span>|<span data-ttu-id="7a1d3-137">String</span><span class="sxs-lookup"><span data-stu-id="7a1d3-137">String</span></span>|<span data-ttu-id="7a1d3-138">ユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-138">User Principal Name.</span></span>|
|<span data-ttu-id="7a1d3-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a1d3-139">installedDeviceCount</span></span>|<span data-ttu-id="7a1d3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7a1d3-140">Int32</span></span>|<span data-ttu-id="7a1d3-141">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-141">Installed Device Count.</span></span>|
|<span data-ttu-id="7a1d3-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a1d3-142">failedDeviceCount</span></span>|<span data-ttu-id="7a1d3-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7a1d3-143">Int32</span></span>|<span data-ttu-id="7a1d3-144">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-144">Failed Device Count.</span></span>|
|<span data-ttu-id="7a1d3-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a1d3-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="7a1d3-146">Int32</span><span class="sxs-lookup"><span data-stu-id="7a1d3-146">Int32</span></span>|<span data-ttu-id="7a1d3-147">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-147">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a1d3-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7a1d3-148">Relationships</span></span>
|<span data-ttu-id="7a1d3-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7a1d3-149">Relationship</span></span>|<span data-ttu-id="7a1d3-150">型</span><span class="sxs-lookup"><span data-stu-id="7a1d3-150">Type</span></span>|<span data-ttu-id="7a1d3-151">説明</span><span class="sxs-lookup"><span data-stu-id="7a1d3-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a1d3-152">アプリ</span><span class="sxs-lookup"><span data-stu-id="7a1d3-152">app</span></span>|[<span data-ttu-id="7a1d3-153">mobileApp</span><span class="sxs-lookup"><span data-stu-id="7a1d3-153">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="7a1d3-154">モバイルアプリへのナビゲーションリンク。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-154">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="7a1d3-155">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="7a1d3-155">deviceStatuses</span></span>|<span data-ttu-id="7a1d3-156">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7a1d3-156">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="7a1d3-157">デバイス上のアプリのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-157">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a1d3-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7a1d3-158">JSON Representation</span></span>
<span data-ttu-id="7a1d3-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7a1d3-159">Here is a JSON representation of the resource.</span></span>
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





