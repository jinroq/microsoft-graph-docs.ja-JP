---
title: userAppInstallStatus リソースの種類
description: ユーザーのインストール状態のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f2d6cd9480cd38653aa35ed8e70705f6fe6ace3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335803"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="62388-103">userAppInstallStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="62388-103">userAppInstallStatus resource type</span></span>

> <span data-ttu-id="62388-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62388-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62388-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="62388-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62388-106">ユーザーのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="62388-106">Contains properties for the installation status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="62388-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="62388-107">Methods</span></span>
|<span data-ttu-id="62388-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="62388-108">Method</span></span>|<span data-ttu-id="62388-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="62388-109">Return Type</span></span>|<span data-ttu-id="62388-110">説明</span><span class="sxs-lookup"><span data-stu-id="62388-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="62388-111">UserAppInstallStatuses 状態を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="62388-111">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="62388-112">[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="62388-112">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="62388-113">[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="62388-113">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="62388-114">UserAppInstallStatus の取得</span><span class="sxs-lookup"><span data-stu-id="62388-114">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="62388-115">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="62388-115">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="62388-116">[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="62388-116">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="62388-117">UserAppInstallStatus の作成</span><span class="sxs-lookup"><span data-stu-id="62388-117">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="62388-118">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="62388-118">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="62388-119">新しい[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="62388-119">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="62388-120">UserAppInstallStatus の削除</span><span class="sxs-lookup"><span data-stu-id="62388-120">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="62388-121">None</span><span class="sxs-lookup"><span data-stu-id="62388-121">None</span></span>|<span data-ttu-id="62388-122">[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="62388-122">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="62388-123">UserAppInstallStatus の更新</span><span class="sxs-lookup"><span data-stu-id="62388-123">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="62388-124">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="62388-124">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="62388-125">[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="62388-125">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="62388-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62388-126">Properties</span></span>
|<span data-ttu-id="62388-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62388-127">Property</span></span>|<span data-ttu-id="62388-128">型</span><span class="sxs-lookup"><span data-stu-id="62388-128">Type</span></span>|<span data-ttu-id="62388-129">説明</span><span class="sxs-lookup"><span data-stu-id="62388-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62388-130">id</span><span class="sxs-lookup"><span data-stu-id="62388-130">id</span></span>|<span data-ttu-id="62388-131">文字列</span><span class="sxs-lookup"><span data-stu-id="62388-131">String</span></span>|<span data-ttu-id="62388-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="62388-132">Key of the entity.</span></span>|
|<span data-ttu-id="62388-133">userName</span><span class="sxs-lookup"><span data-stu-id="62388-133">userName</span></span>|<span data-ttu-id="62388-134">String</span><span class="sxs-lookup"><span data-stu-id="62388-134">String</span></span>|<span data-ttu-id="62388-135">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="62388-135">User name.</span></span>|
|<span data-ttu-id="62388-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="62388-136">userPrincipalName</span></span>|<span data-ttu-id="62388-137">String</span><span class="sxs-lookup"><span data-stu-id="62388-137">String</span></span>|<span data-ttu-id="62388-138">ユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="62388-138">User Principal Name.</span></span>|
|<span data-ttu-id="62388-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="62388-139">installedDeviceCount</span></span>|<span data-ttu-id="62388-140">Int32</span><span class="sxs-lookup"><span data-stu-id="62388-140">Int32</span></span>|<span data-ttu-id="62388-141">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="62388-141">Installed Device Count.</span></span>|
|<span data-ttu-id="62388-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="62388-142">failedDeviceCount</span></span>|<span data-ttu-id="62388-143">Int32</span><span class="sxs-lookup"><span data-stu-id="62388-143">Int32</span></span>|<span data-ttu-id="62388-144">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="62388-144">Failed Device Count.</span></span>|
|<span data-ttu-id="62388-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="62388-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="62388-146">Int32</span><span class="sxs-lookup"><span data-stu-id="62388-146">Int32</span></span>|<span data-ttu-id="62388-147">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="62388-147">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62388-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="62388-148">Relationships</span></span>
|<span data-ttu-id="62388-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="62388-149">Relationship</span></span>|<span data-ttu-id="62388-150">型</span><span class="sxs-lookup"><span data-stu-id="62388-150">Type</span></span>|<span data-ttu-id="62388-151">説明</span><span class="sxs-lookup"><span data-stu-id="62388-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62388-152">アプリ</span><span class="sxs-lookup"><span data-stu-id="62388-152">app</span></span>|[<span data-ttu-id="62388-153">mobileApp</span><span class="sxs-lookup"><span data-stu-id="62388-153">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="62388-154">モバイルアプリへのナビゲーションリンク。</span><span class="sxs-lookup"><span data-stu-id="62388-154">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="62388-155">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="62388-155">deviceStatuses</span></span>|<span data-ttu-id="62388-156">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="62388-156">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="62388-157">デバイス上のアプリのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="62388-157">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62388-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="62388-158">JSON Representation</span></span>
<span data-ttu-id="62388-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="62388-159">Here is a JSON representation of the resource.</span></span>
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



