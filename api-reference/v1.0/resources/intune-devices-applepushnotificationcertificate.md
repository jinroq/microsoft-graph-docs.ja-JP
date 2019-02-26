---
title: applePushNotificationCertificate リソースの種類
description: Apple プッシュ通知証明書。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 41d5161f1e9344f187329bf795219151c91f29ae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256176"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="4d9db-103">applePushNotificationCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4d9db-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="4d9db-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4d9db-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d9db-105">Apple プッシュ通知証明書。</span><span class="sxs-lookup"><span data-stu-id="4d9db-105">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="4d9db-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="4d9db-106">Methods</span></span>
|<span data-ttu-id="4d9db-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4d9db-107">Method</span></span>|<span data-ttu-id="4d9db-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4d9db-108">Return Type</span></span>|<span data-ttu-id="4d9db-109">説明</span><span class="sxs-lookup"><span data-stu-id="4d9db-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4d9db-110">Get applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="4d9db-110">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="4d9db-111">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="4d9db-111">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="4d9db-112">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4d9db-112">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="4d9db-113">Update applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="4d9db-113">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="4d9db-114">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="4d9db-114">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="4d9db-115">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4d9db-115">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="4d9db-116">downloadApplePushNotificationCertificateSigningRequest 関数</span><span class="sxs-lookup"><span data-stu-id="4d9db-116">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="4d9db-117">String</span><span class="sxs-lookup"><span data-stu-id="4d9db-117">String</span></span>|<span data-ttu-id="4d9db-118">Apple プッシュ通知の証明書署名要求をダウンロードします</span><span class="sxs-lookup"><span data-stu-id="4d9db-118">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="4d9db-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d9db-119">Properties</span></span>
|<span data-ttu-id="4d9db-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d9db-120">Property</span></span>|<span data-ttu-id="4d9db-121">型</span><span class="sxs-lookup"><span data-stu-id="4d9db-121">Type</span></span>|<span data-ttu-id="4d9db-122">説明</span><span class="sxs-lookup"><span data-stu-id="4d9db-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d9db-123">id</span><span class="sxs-lookup"><span data-stu-id="4d9db-123">id</span></span>|<span data-ttu-id="4d9db-124">String</span><span class="sxs-lookup"><span data-stu-id="4d9db-124">String</span></span>|<span data-ttu-id="4d9db-125">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="4d9db-125">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="4d9db-126">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="4d9db-126">appleIdentifier</span></span>|<span data-ttu-id="4d9db-127">String</span><span class="sxs-lookup"><span data-stu-id="4d9db-127">String</span></span>|<span data-ttu-id="4d9db-128">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="4d9db-128">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="4d9db-129">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="4d9db-129">topicIdentifier</span></span>|<span data-ttu-id="4d9db-130">String</span><span class="sxs-lookup"><span data-stu-id="4d9db-130">String</span></span>|<span data-ttu-id="4d9db-131">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="4d9db-131">Topic Id.</span></span>|
|<span data-ttu-id="4d9db-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d9db-132">lastModifiedDateTime</span></span>|<span data-ttu-id="4d9db-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d9db-133">DateTimeOffset</span></span>|<span data-ttu-id="4d9db-134">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="4d9db-134">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="4d9db-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4d9db-135">expirationDateTime</span></span>|<span data-ttu-id="4d9db-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d9db-136">DateTimeOffset</span></span>|<span data-ttu-id="4d9db-137">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="4d9db-137">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="4d9db-138">証明書</span><span class="sxs-lookup"><span data-stu-id="4d9db-138">certificate</span></span>|<span data-ttu-id="4d9db-139">String</span><span class="sxs-lookup"><span data-stu-id="4d9db-139">String</span></span>|<span data-ttu-id="4d9db-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4d9db-140">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d9db-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4d9db-141">Relationships</span></span>
<span data-ttu-id="4d9db-142">なし</span><span class="sxs-lookup"><span data-stu-id="4d9db-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d9db-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4d9db-143">JSON Representation</span></span>
<span data-ttu-id="4d9db-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4d9db-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificate": "String"
}
```



