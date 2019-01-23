---
title: userAppInstallStatus リソースの種類
description: プロパティには、ユーザーのインストールのステータスが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1e1369e35af2343bebd609c760075a830649a1f2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399893"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="c2166-103">userAppInstallStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c2166-103">userAppInstallStatus resource type</span></span>

> <span data-ttu-id="c2166-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c2166-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c2166-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2166-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2166-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c2166-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2166-107">プロパティには、ユーザーのインストールのステータスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c2166-107">Contains properties for the installation status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="c2166-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c2166-108">Methods</span></span>
|<span data-ttu-id="c2166-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c2166-109">Method</span></span>|<span data-ttu-id="c2166-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c2166-110">Return Type</span></span>|<span data-ttu-id="c2166-111">説明</span><span class="sxs-lookup"><span data-stu-id="c2166-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c2166-112">リスト userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="c2166-112">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="c2166-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c2166-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="c2166-114">[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c2166-114">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="c2166-115">UserAppInstallStatus を取得します。</span><span class="sxs-lookup"><span data-stu-id="c2166-115">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="c2166-116">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="c2166-116">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="c2166-117">[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2166-117">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="c2166-118">UserAppInstallStatus を作成します。</span><span class="sxs-lookup"><span data-stu-id="c2166-118">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="c2166-119">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="c2166-119">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="c2166-120">新しい[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c2166-120">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="c2166-121">UserAppInstallStatus を削除します。</span><span class="sxs-lookup"><span data-stu-id="c2166-121">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="c2166-122">なし</span><span class="sxs-lookup"><span data-stu-id="c2166-122">None</span></span>|<span data-ttu-id="c2166-123">の[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c2166-123">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="c2166-124">UserAppInstallStatus を更新します。</span><span class="sxs-lookup"><span data-stu-id="c2166-124">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="c2166-125">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="c2166-125">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="c2166-126">[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c2166-126">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c2166-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2166-127">Properties</span></span>
|<span data-ttu-id="c2166-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2166-128">Property</span></span>|<span data-ttu-id="c2166-129">型</span><span class="sxs-lookup"><span data-stu-id="c2166-129">Type</span></span>|<span data-ttu-id="c2166-130">説明</span><span class="sxs-lookup"><span data-stu-id="c2166-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2166-131">id</span><span class="sxs-lookup"><span data-stu-id="c2166-131">id</span></span>|<span data-ttu-id="c2166-132">String</span><span class="sxs-lookup"><span data-stu-id="c2166-132">String</span></span>|<span data-ttu-id="c2166-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c2166-133">Key of the entity.</span></span>|
|<span data-ttu-id="c2166-134">userName</span><span class="sxs-lookup"><span data-stu-id="c2166-134">userName</span></span>|<span data-ttu-id="c2166-135">String</span><span class="sxs-lookup"><span data-stu-id="c2166-135">String</span></span>|<span data-ttu-id="c2166-136">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="c2166-136">User name.</span></span>|
|<span data-ttu-id="c2166-137">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c2166-137">userPrincipalName</span></span>|<span data-ttu-id="c2166-138">String</span><span class="sxs-lookup"><span data-stu-id="c2166-138">String</span></span>|<span data-ttu-id="c2166-139">ユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="c2166-139">User Principal Name.</span></span>|
|<span data-ttu-id="c2166-140">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c2166-140">installedDeviceCount</span></span>|<span data-ttu-id="c2166-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c2166-141">Int32</span></span>|<span data-ttu-id="c2166-142">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="c2166-142">Installed Device Count.</span></span>|
|<span data-ttu-id="c2166-143">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c2166-143">failedDeviceCount</span></span>|<span data-ttu-id="c2166-144">Int32</span><span class="sxs-lookup"><span data-stu-id="c2166-144">Int32</span></span>|<span data-ttu-id="c2166-145">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="c2166-145">Failed Device Count.</span></span>|
|<span data-ttu-id="c2166-146">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c2166-146">notInstalledDeviceCount</span></span>|<span data-ttu-id="c2166-147">Int32</span><span class="sxs-lookup"><span data-stu-id="c2166-147">Int32</span></span>|<span data-ttu-id="c2166-148">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="c2166-148">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2166-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c2166-149">Relationships</span></span>
|<span data-ttu-id="c2166-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c2166-150">Relationship</span></span>|<span data-ttu-id="c2166-151">型</span><span class="sxs-lookup"><span data-stu-id="c2166-151">Type</span></span>|<span data-ttu-id="c2166-152">説明</span><span class="sxs-lookup"><span data-stu-id="c2166-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2166-153">アプリ</span><span class="sxs-lookup"><span data-stu-id="c2166-153">app</span></span>|[<span data-ttu-id="c2166-154">mobileApp</span><span class="sxs-lookup"><span data-stu-id="c2166-154">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="c2166-155">モバイル アプリケーションへのナビゲーション リンクです。</span><span class="sxs-lookup"><span data-stu-id="c2166-155">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="c2166-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c2166-156">deviceStatuses</span></span>|<span data-ttu-id="c2166-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c2166-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="c2166-158">デバイス上のアプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="c2166-158">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2166-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c2166-159">JSON Representation</span></span>
<span data-ttu-id="c2166-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c2166-160">Here is a JSON representation of the resource.</span></span>
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




