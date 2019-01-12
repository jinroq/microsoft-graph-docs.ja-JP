---
title: eBookInstallSummary リソース タイプ
description: デバイスのブックのインストール要約のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a3d07dc2d1a1b7a117e001546cd5298765676bdd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986153"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="13ff5-103">eBookInstallSummary リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="13ff5-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="13ff5-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="13ff5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13ff5-105">デバイスのブックのインストール要約のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="13ff5-105">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="13ff5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="13ff5-106">Methods</span></span>
|<span data-ttu-id="13ff5-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="13ff5-107">Method</span></span>|<span data-ttu-id="13ff5-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="13ff5-108">Return Type</span></span>|<span data-ttu-id="13ff5-109">説明</span><span class="sxs-lookup"><span data-stu-id="13ff5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13ff5-110">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="13ff5-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="13ff5-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="13ff5-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="13ff5-112">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="13ff5-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="13ff5-113">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="13ff5-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="13ff5-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="13ff5-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="13ff5-115">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="13ff5-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="13ff5-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13ff5-116">Properties</span></span>
|<span data-ttu-id="13ff5-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13ff5-117">Property</span></span>|<span data-ttu-id="13ff5-118">種類</span><span class="sxs-lookup"><span data-stu-id="13ff5-118">Type</span></span>|<span data-ttu-id="13ff5-119">説明</span><span class="sxs-lookup"><span data-stu-id="13ff5-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13ff5-120">ID</span><span class="sxs-lookup"><span data-stu-id="13ff5-120">id</span></span>|<span data-ttu-id="13ff5-121">String</span><span class="sxs-lookup"><span data-stu-id="13ff5-121">String</span></span>|<span data-ttu-id="13ff5-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="13ff5-122">Key of the entity.</span></span>|
|<span data-ttu-id="13ff5-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="13ff5-123">installedDeviceCount</span></span>|<span data-ttu-id="13ff5-124">Int32</span><span class="sxs-lookup"><span data-stu-id="13ff5-124">Int32</span></span>|<span data-ttu-id="13ff5-125">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="13ff5-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="13ff5-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="13ff5-126">failedDeviceCount</span></span>|<span data-ttu-id="13ff5-127">Int32</span><span class="sxs-lookup"><span data-stu-id="13ff5-127">Int32</span></span>|<span data-ttu-id="13ff5-128">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="13ff5-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="13ff5-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="13ff5-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="13ff5-130">Int32</span><span class="sxs-lookup"><span data-stu-id="13ff5-130">Int32</span></span>|<span data-ttu-id="13ff5-131">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="13ff5-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="13ff5-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="13ff5-132">installedUserCount</span></span>|<span data-ttu-id="13ff5-133">Int32</span><span class="sxs-lookup"><span data-stu-id="13ff5-133">Int32</span></span>|<span data-ttu-id="13ff5-134">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="13ff5-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="13ff5-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="13ff5-135">failedUserCount</span></span>|<span data-ttu-id="13ff5-136">Int32</span><span class="sxs-lookup"><span data-stu-id="13ff5-136">Int32</span></span>|<span data-ttu-id="13ff5-137">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="13ff5-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="13ff5-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="13ff5-138">notInstalledUserCount</span></span>|<span data-ttu-id="13ff5-139">Int32</span><span class="sxs-lookup"><span data-stu-id="13ff5-139">Int32</span></span>|<span data-ttu-id="13ff5-140">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="13ff5-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13ff5-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="13ff5-141">Relationships</span></span>
<span data-ttu-id="13ff5-142">なし</span><span class="sxs-lookup"><span data-stu-id="13ff5-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="13ff5-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13ff5-143">JSON Representation</span></span>
<span data-ttu-id="13ff5-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="13ff5-144">Here is a JSON representation of the resource.</span></span>
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



