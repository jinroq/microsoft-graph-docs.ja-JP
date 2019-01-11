---
title: userInstallStateSummary リソースの種類
description: ユーザーのインストール状態の要約のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c87ca0ab41a95a6a1d214e83eb94a03a4f2330a4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820770"
---
# <a name="userinstallstatesummary-resource-type"></a><span data-ttu-id="6b6b8-103">userInstallStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6b6b8-103">userInstallStateSummary resource type</span></span>

> <span data-ttu-id="6b6b8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b6b8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b6b8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b6b8-107">ユーザーのインストール状態の要約のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-107">Contains properties for the installation state summary for a user.</span></span>
## <a name="methods"></a><span data-ttu-id="6b6b8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6b6b8-108">Methods</span></span>
|<span data-ttu-id="6b6b8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6b6b8-109">Method</span></span>|<span data-ttu-id="6b6b8-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6b6b8-110">Return Type</span></span>|<span data-ttu-id="6b6b8-111">説明</span><span class="sxs-lookup"><span data-stu-id="6b6b8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6b6b8-112">userInstallStateSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="6b6b8-112">List userInstallStateSummaries</span></span>](../api/intune-books-userinstallstatesummary-list.md)|<span data-ttu-id="6b6b8-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b6b8-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="6b6b8-114">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-114">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="6b6b8-115">userInstallStateSummary の取得</span><span class="sxs-lookup"><span data-stu-id="6b6b8-115">Get userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-get.md)|[<span data-ttu-id="6b6b8-116">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="6b6b8-116">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="6b6b8-117">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-117">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="6b6b8-118">userInstallStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="6b6b8-118">Create userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-create.md)|[<span data-ttu-id="6b6b8-119">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="6b6b8-119">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="6b6b8-120">新しい [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-120">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="6b6b8-121">userInstallStateSummary の削除</span><span class="sxs-lookup"><span data-stu-id="6b6b8-121">Delete userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-delete.md)|<span data-ttu-id="6b6b8-122">なし</span><span class="sxs-lookup"><span data-stu-id="6b6b8-122">None</span></span>|<span data-ttu-id="6b6b8-123">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-123">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>|
|[<span data-ttu-id="6b6b8-124">userInstallStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="6b6b8-124">Update userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-update.md)|[<span data-ttu-id="6b6b8-125">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="6b6b8-125">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="6b6b8-126">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-126">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6b6b8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b6b8-127">Properties</span></span>
|<span data-ttu-id="6b6b8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b6b8-128">Property</span></span>|<span data-ttu-id="6b6b8-129">種類</span><span class="sxs-lookup"><span data-stu-id="6b6b8-129">Type</span></span>|<span data-ttu-id="6b6b8-130">説明</span><span class="sxs-lookup"><span data-stu-id="6b6b8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b6b8-131">ID</span><span class="sxs-lookup"><span data-stu-id="6b6b8-131">id</span></span>|<span data-ttu-id="6b6b8-132">String</span><span class="sxs-lookup"><span data-stu-id="6b6b8-132">String</span></span>|<span data-ttu-id="6b6b8-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-133">Key of the entity.</span></span>|
|<span data-ttu-id="6b6b8-134">userName</span><span class="sxs-lookup"><span data-stu-id="6b6b8-134">userName</span></span>|<span data-ttu-id="6b6b8-135">String</span><span class="sxs-lookup"><span data-stu-id="6b6b8-135">String</span></span>|<span data-ttu-id="6b6b8-136">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-136">User name.</span></span>|
|<span data-ttu-id="6b6b8-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b6b8-137">installedDeviceCount</span></span>|<span data-ttu-id="6b6b8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="6b6b8-138">Int32</span></span>|<span data-ttu-id="6b6b8-139">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-139">Installed Device Count.</span></span>|
|<span data-ttu-id="6b6b8-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b6b8-140">failedDeviceCount</span></span>|<span data-ttu-id="6b6b8-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6b6b8-141">Int32</span></span>|<span data-ttu-id="6b6b8-142">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-142">Failed Device Count.</span></span>|
|<span data-ttu-id="6b6b8-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b6b8-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="6b6b8-144">Int32</span><span class="sxs-lookup"><span data-stu-id="6b6b8-144">Int32</span></span>|<span data-ttu-id="6b6b8-145">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-145">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b6b8-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6b6b8-146">Relationships</span></span>
|<span data-ttu-id="6b6b8-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6b6b8-147">Relationship</span></span>|<span data-ttu-id="6b6b8-148">型</span><span class="sxs-lookup"><span data-stu-id="6b6b8-148">Type</span></span>|<span data-ttu-id="6b6b8-149">説明</span><span class="sxs-lookup"><span data-stu-id="6b6b8-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b6b8-150">deviceStates</span><span class="sxs-lookup"><span data-stu-id="6b6b8-150">deviceStates</span></span>|<span data-ttu-id="6b6b8-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b6b8-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="6b6b8-152">電子ブックのインストールの状態です。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-152">The install state of the eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b6b8-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6b6b8-153">JSON Representation</span></span>
<span data-ttu-id="6b6b8-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6b6b8-154">Here is a JSON representation of the resource.</span></span>
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





