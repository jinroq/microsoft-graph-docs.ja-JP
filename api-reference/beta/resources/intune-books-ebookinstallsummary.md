---
title: eBookInstallSummary リソース タイプ
description: デバイスのブックのインストール要約のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d3a5d1ce5c05d0a8c20a79aea2fd3562ab2170c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915943"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="7ac3f-103">eBookInstallSummary リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="7ac3f-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="7ac3f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7ac3f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ac3f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ac3f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ac3f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ac3f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ac3f-107">デバイスのブックのインストール要約のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7ac3f-107">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="7ac3f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7ac3f-108">Methods</span></span>
|<span data-ttu-id="7ac3f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="7ac3f-109">Method</span></span>|<span data-ttu-id="7ac3f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7ac3f-110">Return Type</span></span>|<span data-ttu-id="7ac3f-111">説明</span><span class="sxs-lookup"><span data-stu-id="7ac3f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7ac3f-112">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7ac3f-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="7ac3f-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7ac3f-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="7ac3f-114">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7ac3f-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="7ac3f-115">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7ac3f-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="7ac3f-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7ac3f-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="7ac3f-117">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7ac3f-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7ac3f-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ac3f-118">Properties</span></span>
|<span data-ttu-id="7ac3f-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ac3f-119">Property</span></span>|<span data-ttu-id="7ac3f-120">型</span><span class="sxs-lookup"><span data-stu-id="7ac3f-120">Type</span></span>|<span data-ttu-id="7ac3f-121">説明</span><span class="sxs-lookup"><span data-stu-id="7ac3f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ac3f-122">ID</span><span class="sxs-lookup"><span data-stu-id="7ac3f-122">id</span></span>|<span data-ttu-id="7ac3f-123">String</span><span class="sxs-lookup"><span data-stu-id="7ac3f-123">String</span></span>|<span data-ttu-id="7ac3f-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7ac3f-124">Key of the entity.</span></span>|
|<span data-ttu-id="7ac3f-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ac3f-125">installedDeviceCount</span></span>|<span data-ttu-id="7ac3f-126">Int32</span><span class="sxs-lookup"><span data-stu-id="7ac3f-126">Int32</span></span>|<span data-ttu-id="7ac3f-127">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="7ac3f-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="7ac3f-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ac3f-128">failedDeviceCount</span></span>|<span data-ttu-id="7ac3f-129">Int32</span><span class="sxs-lookup"><span data-stu-id="7ac3f-129">Int32</span></span>|<span data-ttu-id="7ac3f-130">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="7ac3f-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="7ac3f-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ac3f-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="7ac3f-132">Int32</span><span class="sxs-lookup"><span data-stu-id="7ac3f-132">Int32</span></span>|<span data-ttu-id="7ac3f-133">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="7ac3f-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="7ac3f-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="7ac3f-134">installedUserCount</span></span>|<span data-ttu-id="7ac3f-135">Int32</span><span class="sxs-lookup"><span data-stu-id="7ac3f-135">Int32</span></span>|<span data-ttu-id="7ac3f-136">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="7ac3f-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="7ac3f-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="7ac3f-137">failedUserCount</span></span>|<span data-ttu-id="7ac3f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7ac3f-138">Int32</span></span>|<span data-ttu-id="7ac3f-139">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="7ac3f-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="7ac3f-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="7ac3f-140">notInstalledUserCount</span></span>|<span data-ttu-id="7ac3f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="7ac3f-141">Int32</span></span>|<span data-ttu-id="7ac3f-142">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="7ac3f-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ac3f-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7ac3f-143">Relationships</span></span>
<span data-ttu-id="7ac3f-144">なし</span><span class="sxs-lookup"><span data-stu-id="7ac3f-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7ac3f-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7ac3f-145">JSON Representation</span></span>
<span data-ttu-id="7ac3f-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7ac3f-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```





