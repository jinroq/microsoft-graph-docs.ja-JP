---
title: userAppInstallStatus リソースの種類
description: プロパティには、ユーザーのインストールのステータスが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f17a504537b1230de175e033779441627f5f98be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938014"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="759cb-103">userAppInstallStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="759cb-103">userAppInstallStatus resource type</span></span>

> <span data-ttu-id="759cb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="759cb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="759cb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="759cb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="759cb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="759cb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="759cb-107">プロパティには、ユーザーのインストールのステータスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="759cb-107">Contains properties for the installation status for a user.</span></span>
## <a name="methods"></a><span data-ttu-id="759cb-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="759cb-108">Methods</span></span>
|<span data-ttu-id="759cb-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="759cb-109">Method</span></span>|<span data-ttu-id="759cb-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="759cb-110">Return Type</span></span>|<span data-ttu-id="759cb-111">説明</span><span class="sxs-lookup"><span data-stu-id="759cb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="759cb-112">リスト userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="759cb-112">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="759cb-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="759cb-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="759cb-114">[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="759cb-114">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="759cb-115">UserAppInstallStatus を取得します。</span><span class="sxs-lookup"><span data-stu-id="759cb-115">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="759cb-116">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="759cb-116">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="759cb-117">[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="759cb-117">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="759cb-118">UserAppInstallStatus を作成します。</span><span class="sxs-lookup"><span data-stu-id="759cb-118">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="759cb-119">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="759cb-119">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="759cb-120">新しい[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="759cb-120">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="759cb-121">UserAppInstallStatus を削除します。</span><span class="sxs-lookup"><span data-stu-id="759cb-121">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="759cb-122">なし</span><span class="sxs-lookup"><span data-stu-id="759cb-122">None</span></span>|<span data-ttu-id="759cb-123">の[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="759cb-123">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="759cb-124">UserAppInstallStatus を更新します。</span><span class="sxs-lookup"><span data-stu-id="759cb-124">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="759cb-125">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="759cb-125">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="759cb-126">[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="759cb-126">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="759cb-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="759cb-127">Properties</span></span>
|<span data-ttu-id="759cb-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="759cb-128">Property</span></span>|<span data-ttu-id="759cb-129">型</span><span class="sxs-lookup"><span data-stu-id="759cb-129">Type</span></span>|<span data-ttu-id="759cb-130">説明</span><span class="sxs-lookup"><span data-stu-id="759cb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="759cb-131">ID</span><span class="sxs-lookup"><span data-stu-id="759cb-131">id</span></span>|<span data-ttu-id="759cb-132">String</span><span class="sxs-lookup"><span data-stu-id="759cb-132">String</span></span>|<span data-ttu-id="759cb-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="759cb-133">Key of the entity.</span></span>|
|<span data-ttu-id="759cb-134">userName</span><span class="sxs-lookup"><span data-stu-id="759cb-134">userName</span></span>|<span data-ttu-id="759cb-135">String</span><span class="sxs-lookup"><span data-stu-id="759cb-135">String</span></span>|<span data-ttu-id="759cb-136">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="759cb-136">User name.</span></span>|
|<span data-ttu-id="759cb-137">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="759cb-137">userPrincipalName</span></span>|<span data-ttu-id="759cb-138">String</span><span class="sxs-lookup"><span data-stu-id="759cb-138">String</span></span>|<span data-ttu-id="759cb-139">ユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="759cb-139">User Principal Name.</span></span>|
|<span data-ttu-id="759cb-140">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="759cb-140">installedDeviceCount</span></span>|<span data-ttu-id="759cb-141">Int32</span><span class="sxs-lookup"><span data-stu-id="759cb-141">Int32</span></span>|<span data-ttu-id="759cb-142">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="759cb-142">Installed Device Count.</span></span>|
|<span data-ttu-id="759cb-143">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="759cb-143">failedDeviceCount</span></span>|<span data-ttu-id="759cb-144">Int32</span><span class="sxs-lookup"><span data-stu-id="759cb-144">Int32</span></span>|<span data-ttu-id="759cb-145">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="759cb-145">Failed Device Count.</span></span>|
|<span data-ttu-id="759cb-146">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="759cb-146">notInstalledDeviceCount</span></span>|<span data-ttu-id="759cb-147">Int32</span><span class="sxs-lookup"><span data-stu-id="759cb-147">Int32</span></span>|<span data-ttu-id="759cb-148">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="759cb-148">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="759cb-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="759cb-149">Relationships</span></span>
|<span data-ttu-id="759cb-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="759cb-150">Relationship</span></span>|<span data-ttu-id="759cb-151">型</span><span class="sxs-lookup"><span data-stu-id="759cb-151">Type</span></span>|<span data-ttu-id="759cb-152">説明</span><span class="sxs-lookup"><span data-stu-id="759cb-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="759cb-153">アプリ</span><span class="sxs-lookup"><span data-stu-id="759cb-153">app</span></span>|[<span data-ttu-id="759cb-154">mobileApp</span><span class="sxs-lookup"><span data-stu-id="759cb-154">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="759cb-155">モバイル アプリケーションへのナビゲーション リンクです。</span><span class="sxs-lookup"><span data-stu-id="759cb-155">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="759cb-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="759cb-156">deviceStatuses</span></span>|<span data-ttu-id="759cb-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="759cb-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="759cb-158">デバイス上のアプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="759cb-158">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="759cb-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="759cb-159">JSON Representation</span></span>
<span data-ttu-id="759cb-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="759cb-160">Here is a JSON representation of the resource.</span></span>
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





