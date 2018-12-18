---
title: eBookInstallSummary リソース タイプ
description: デバイスのブックのインストール要約のプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: 4f94c82a0d7cd234206586829981c62ba7d0a959
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344276"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="40d5a-103">eBookInstallSummary リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="40d5a-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="40d5a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="40d5a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40d5a-105">デバイスのブックのインストール要約のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="40d5a-105">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="40d5a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="40d5a-106">Methods</span></span>
|<span data-ttu-id="40d5a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="40d5a-107">Method</span></span>|<span data-ttu-id="40d5a-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="40d5a-108">Return Type</span></span>|<span data-ttu-id="40d5a-109">説明</span><span class="sxs-lookup"><span data-stu-id="40d5a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="40d5a-110">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="40d5a-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="40d5a-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="40d5a-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="40d5a-112">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="40d5a-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="40d5a-113">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="40d5a-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="40d5a-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="40d5a-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="40d5a-115">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="40d5a-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="40d5a-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40d5a-116">Properties</span></span>
|<span data-ttu-id="40d5a-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40d5a-117">Property</span></span>|<span data-ttu-id="40d5a-118">種類</span><span class="sxs-lookup"><span data-stu-id="40d5a-118">Type</span></span>|<span data-ttu-id="40d5a-119">説明</span><span class="sxs-lookup"><span data-stu-id="40d5a-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40d5a-120">ID</span><span class="sxs-lookup"><span data-stu-id="40d5a-120">id</span></span>|<span data-ttu-id="40d5a-121">String</span><span class="sxs-lookup"><span data-stu-id="40d5a-121">String</span></span>|<span data-ttu-id="40d5a-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="40d5a-122">Key of the entity.</span></span>|
|<span data-ttu-id="40d5a-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="40d5a-123">installedDeviceCount</span></span>|<span data-ttu-id="40d5a-124">Int32</span><span class="sxs-lookup"><span data-stu-id="40d5a-124">Int32</span></span>|<span data-ttu-id="40d5a-125">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="40d5a-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="40d5a-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="40d5a-126">failedDeviceCount</span></span>|<span data-ttu-id="40d5a-127">Int32</span><span class="sxs-lookup"><span data-stu-id="40d5a-127">Int32</span></span>|<span data-ttu-id="40d5a-128">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="40d5a-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="40d5a-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="40d5a-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="40d5a-130">Int32</span><span class="sxs-lookup"><span data-stu-id="40d5a-130">Int32</span></span>|<span data-ttu-id="40d5a-131">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="40d5a-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="40d5a-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="40d5a-132">installedUserCount</span></span>|<span data-ttu-id="40d5a-133">Int32</span><span class="sxs-lookup"><span data-stu-id="40d5a-133">Int32</span></span>|<span data-ttu-id="40d5a-134">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="40d5a-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="40d5a-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="40d5a-135">failedUserCount</span></span>|<span data-ttu-id="40d5a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="40d5a-136">Int32</span></span>|<span data-ttu-id="40d5a-137">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="40d5a-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="40d5a-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="40d5a-138">notInstalledUserCount</span></span>|<span data-ttu-id="40d5a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="40d5a-139">Int32</span></span>|<span data-ttu-id="40d5a-140">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="40d5a-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40d5a-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="40d5a-141">Relationships</span></span>
<span data-ttu-id="40d5a-142">なし</span><span class="sxs-lookup"><span data-stu-id="40d5a-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="40d5a-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="40d5a-143">JSON Representation</span></span>
<span data-ttu-id="40d5a-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="40d5a-144">Here is a JSON representation of the resource.</span></span>
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



