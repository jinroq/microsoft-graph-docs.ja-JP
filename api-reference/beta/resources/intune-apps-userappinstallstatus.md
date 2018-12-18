---
title: userAppInstallStatus リソースの種類
description: プロパティには、ユーザーのインストールのステータスが含まれています。
author: tfitzmac
ms.openlocfilehash: 024fff32aac2a268a2e0bbec81a6d46b31012a11
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302759"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="8fe34-103">userAppInstallStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8fe34-103">userAppInstallStatus resource type</span></span>

> <span data-ttu-id="8fe34-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8fe34-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fe34-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fe34-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8fe34-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8fe34-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fe34-107">プロパティには、ユーザーのインストールのステータスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8fe34-107">Contains properties for the installation status for a user.</span></span>
## <a name="methods"></a><span data-ttu-id="8fe34-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8fe34-108">Methods</span></span>
|<span data-ttu-id="8fe34-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="8fe34-109">Method</span></span>|<span data-ttu-id="8fe34-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8fe34-110">Return Type</span></span>|<span data-ttu-id="8fe34-111">説明</span><span class="sxs-lookup"><span data-stu-id="8fe34-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8fe34-112">リスト userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="8fe34-112">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="8fe34-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8fe34-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="8fe34-114">[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8fe34-114">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="8fe34-115">UserAppInstallStatus を取得します。</span><span class="sxs-lookup"><span data-stu-id="8fe34-115">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="8fe34-116">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="8fe34-116">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="8fe34-117">[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8fe34-117">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="8fe34-118">UserAppInstallStatus を作成します。</span><span class="sxs-lookup"><span data-stu-id="8fe34-118">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="8fe34-119">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="8fe34-119">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="8fe34-120">新しい[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8fe34-120">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="8fe34-121">UserAppInstallStatus を削除します。</span><span class="sxs-lookup"><span data-stu-id="8fe34-121">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="8fe34-122">なし</span><span class="sxs-lookup"><span data-stu-id="8fe34-122">None</span></span>|<span data-ttu-id="8fe34-123">の[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="8fe34-123">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="8fe34-124">UserAppInstallStatus を更新します。</span><span class="sxs-lookup"><span data-stu-id="8fe34-124">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="8fe34-125">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="8fe34-125">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="8fe34-126">[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8fe34-126">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8fe34-127">Properties</span><span class="sxs-lookup"><span data-stu-id="8fe34-127">Properties</span></span>
|<span data-ttu-id="8fe34-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fe34-128">Property</span></span>|<span data-ttu-id="8fe34-129">種類</span><span class="sxs-lookup"><span data-stu-id="8fe34-129">Type</span></span>|<span data-ttu-id="8fe34-130">説明</span><span class="sxs-lookup"><span data-stu-id="8fe34-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fe34-131">ID</span><span class="sxs-lookup"><span data-stu-id="8fe34-131">id</span></span>|<span data-ttu-id="8fe34-132">String</span><span class="sxs-lookup"><span data-stu-id="8fe34-132">String</span></span>|<span data-ttu-id="8fe34-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8fe34-133">Key of the entity.</span></span>|
|<span data-ttu-id="8fe34-134">userName</span><span class="sxs-lookup"><span data-stu-id="8fe34-134">userName</span></span>|<span data-ttu-id="8fe34-135">String</span><span class="sxs-lookup"><span data-stu-id="8fe34-135">String</span></span>|<span data-ttu-id="8fe34-136">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="8fe34-136">User name.</span></span>|
|<span data-ttu-id="8fe34-137">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8fe34-137">userPrincipalName</span></span>|<span data-ttu-id="8fe34-138">String</span><span class="sxs-lookup"><span data-stu-id="8fe34-138">String</span></span>|<span data-ttu-id="8fe34-139">ユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="8fe34-139">User Principal Name.</span></span>|
|<span data-ttu-id="8fe34-140">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fe34-140">installedDeviceCount</span></span>|<span data-ttu-id="8fe34-141">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe34-141">Int32</span></span>|<span data-ttu-id="8fe34-142">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="8fe34-142">Installed Device Count.</span></span>|
|<span data-ttu-id="8fe34-143">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fe34-143">failedDeviceCount</span></span>|<span data-ttu-id="8fe34-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe34-144">Int32</span></span>|<span data-ttu-id="8fe34-145">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="8fe34-145">Failed Device Count.</span></span>|
|<span data-ttu-id="8fe34-146">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fe34-146">notInstalledDeviceCount</span></span>|<span data-ttu-id="8fe34-147">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe34-147">Int32</span></span>|<span data-ttu-id="8fe34-148">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="8fe34-148">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fe34-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8fe34-149">Relationships</span></span>
|<span data-ttu-id="8fe34-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8fe34-150">Relationship</span></span>|<span data-ttu-id="8fe34-151">型</span><span class="sxs-lookup"><span data-stu-id="8fe34-151">Type</span></span>|<span data-ttu-id="8fe34-152">説明</span><span class="sxs-lookup"><span data-stu-id="8fe34-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fe34-153">アプリ</span><span class="sxs-lookup"><span data-stu-id="8fe34-153">app</span></span>|[<span data-ttu-id="8fe34-154">mobileApp</span><span class="sxs-lookup"><span data-stu-id="8fe34-154">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="8fe34-155">モバイル アプリケーションへのナビゲーション リンクです。</span><span class="sxs-lookup"><span data-stu-id="8fe34-155">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="8fe34-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="8fe34-156">deviceStatuses</span></span>|<span data-ttu-id="8fe34-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8fe34-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="8fe34-158">デバイス上のアプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="8fe34-158">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8fe34-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8fe34-159">JSON Representation</span></span>
<span data-ttu-id="8fe34-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8fe34-160">Here is a JSON representation of the resource.</span></span>
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





