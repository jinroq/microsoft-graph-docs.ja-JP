---
title: applePushNotificationCertificate リソースの種類
description: Apple プッシュ通知証明書。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9c8d968e48b1aa5e02c554dc8a5392165f0a3f9e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917735"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="ce202-103">applePushNotificationCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce202-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="ce202-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ce202-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce202-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce202-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce202-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce202-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce202-107">Apple プッシュ通知証明書。</span><span class="sxs-lookup"><span data-stu-id="ce202-107">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="ce202-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ce202-108">Methods</span></span>
|<span data-ttu-id="ce202-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ce202-109">Method</span></span>|<span data-ttu-id="ce202-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ce202-110">Return Type</span></span>|<span data-ttu-id="ce202-111">説明</span><span class="sxs-lookup"><span data-stu-id="ce202-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ce202-112">Get applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ce202-112">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="ce202-113">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ce202-113">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="ce202-114">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ce202-114">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="ce202-115">Update applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ce202-115">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="ce202-116">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ce202-116">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="ce202-117">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ce202-117">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="ce202-118">downloadApplePushNotificationCertificateSigningRequest 関数</span><span class="sxs-lookup"><span data-stu-id="ce202-118">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="ce202-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ce202-119">String</span></span>|<span data-ttu-id="ce202-120">Apple プッシュ通知の証明書署名要求をダウンロードします</span><span class="sxs-lookup"><span data-stu-id="ce202-120">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="ce202-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce202-121">Properties</span></span>
|<span data-ttu-id="ce202-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce202-122">Property</span></span>|<span data-ttu-id="ce202-123">種類</span><span class="sxs-lookup"><span data-stu-id="ce202-123">Type</span></span>|<span data-ttu-id="ce202-124">説明</span><span class="sxs-lookup"><span data-stu-id="ce202-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce202-125">ID</span><span class="sxs-lookup"><span data-stu-id="ce202-125">id</span></span>|<span data-ttu-id="ce202-126">String</span><span class="sxs-lookup"><span data-stu-id="ce202-126">String</span></span>|<span data-ttu-id="ce202-127">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="ce202-127">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="ce202-128">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="ce202-128">appleIdentifier</span></span>|<span data-ttu-id="ce202-129">String</span><span class="sxs-lookup"><span data-stu-id="ce202-129">String</span></span>|<span data-ttu-id="ce202-130">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="ce202-130">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="ce202-131">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="ce202-131">topicIdentifier</span></span>|<span data-ttu-id="ce202-132">String</span><span class="sxs-lookup"><span data-stu-id="ce202-132">String</span></span>|<span data-ttu-id="ce202-133">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="ce202-133">Topic Id.</span></span>|
|<span data-ttu-id="ce202-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce202-134">lastModifiedDateTime</span></span>|<span data-ttu-id="ce202-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce202-135">DateTimeOffset</span></span>|<span data-ttu-id="ce202-136">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="ce202-136">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="ce202-137">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ce202-137">expirationDateTime</span></span>|<span data-ttu-id="ce202-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce202-138">DateTimeOffset</span></span>|<span data-ttu-id="ce202-139">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="ce202-139">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="ce202-140">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="ce202-140">certificateUploadStatus</span></span>|<span data-ttu-id="ce202-141">String</span><span class="sxs-lookup"><span data-stu-id="ce202-141">String</span></span>|<span data-ttu-id="ce202-142">証明書のアップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="ce202-142">The certificate upload status.</span></span>|
|<span data-ttu-id="ce202-143">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="ce202-143">certificateUploadFailureReason</span></span>|<span data-ttu-id="ce202-144">String</span><span class="sxs-lookup"><span data-stu-id="ce202-144">String</span></span>|<span data-ttu-id="ce202-145">理由の証明書のアップロードに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="ce202-145">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="ce202-146">証明書</span><span class="sxs-lookup"><span data-stu-id="ce202-146">certificate</span></span>|<span data-ttu-id="ce202-147">String</span><span class="sxs-lookup"><span data-stu-id="ce202-147">String</span></span>|<span data-ttu-id="ce202-148">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ce202-148">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce202-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ce202-149">Relationships</span></span>
<span data-ttu-id="ce202-150">なし</span><span class="sxs-lookup"><span data-stu-id="ce202-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ce202-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce202-151">JSON Representation</span></span>
<span data-ttu-id="ce202-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ce202-152">Here is a JSON representation of the resource.</span></span>
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
  "certificateUploadStatus": "String",
  "certificateUploadFailureReason": "String",
  "certificate": "String"
}
```





