---
title: applePushNotificationCertificate リソースの種類
description: Apple プッシュ通知証明書。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3cc0b4a3e35027f79dd79ab065de9632e9585873
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810865"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="f8b2f-103">applePushNotificationCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f8b2f-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="f8b2f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f8b2f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8b2f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8b2f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8b2f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f8b2f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8b2f-107">Apple プッシュ通知証明書。</span><span class="sxs-lookup"><span data-stu-id="f8b2f-107">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="f8b2f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f8b2f-108">Methods</span></span>
|<span data-ttu-id="f8b2f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="f8b2f-109">Method</span></span>|<span data-ttu-id="f8b2f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f8b2f-110">Return Type</span></span>|<span data-ttu-id="f8b2f-111">説明</span><span class="sxs-lookup"><span data-stu-id="f8b2f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f8b2f-112">Get applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f8b2f-112">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="f8b2f-113">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f8b2f-113">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="f8b2f-114">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f8b2f-114">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="f8b2f-115">Update applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f8b2f-115">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="f8b2f-116">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f8b2f-116">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="f8b2f-117">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f8b2f-117">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="f8b2f-118">downloadApplePushNotificationCertificateSigningRequest 関数</span><span class="sxs-lookup"><span data-stu-id="f8b2f-118">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="f8b2f-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f8b2f-119">String</span></span>|<span data-ttu-id="f8b2f-120">Apple プッシュ通知の証明書署名要求をダウンロードします</span><span class="sxs-lookup"><span data-stu-id="f8b2f-120">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="f8b2f-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8b2f-121">Properties</span></span>
|<span data-ttu-id="f8b2f-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8b2f-122">Property</span></span>|<span data-ttu-id="f8b2f-123">種類</span><span class="sxs-lookup"><span data-stu-id="f8b2f-123">Type</span></span>|<span data-ttu-id="f8b2f-124">説明</span><span class="sxs-lookup"><span data-stu-id="f8b2f-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8b2f-125">ID</span><span class="sxs-lookup"><span data-stu-id="f8b2f-125">id</span></span>|<span data-ttu-id="f8b2f-126">String</span><span class="sxs-lookup"><span data-stu-id="f8b2f-126">String</span></span>|<span data-ttu-id="f8b2f-127">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="f8b2f-127">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="f8b2f-128">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="f8b2f-128">appleIdentifier</span></span>|<span data-ttu-id="f8b2f-129">String</span><span class="sxs-lookup"><span data-stu-id="f8b2f-129">String</span></span>|<span data-ttu-id="f8b2f-130">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="f8b2f-130">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="f8b2f-131">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="f8b2f-131">topicIdentifier</span></span>|<span data-ttu-id="f8b2f-132">String</span><span class="sxs-lookup"><span data-stu-id="f8b2f-132">String</span></span>|<span data-ttu-id="f8b2f-133">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="f8b2f-133">Topic Id.</span></span>|
|<span data-ttu-id="f8b2f-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8b2f-134">lastModifiedDateTime</span></span>|<span data-ttu-id="f8b2f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8b2f-135">DateTimeOffset</span></span>|<span data-ttu-id="f8b2f-136">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="f8b2f-136">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="f8b2f-137">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f8b2f-137">expirationDateTime</span></span>|<span data-ttu-id="f8b2f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8b2f-138">DateTimeOffset</span></span>|<span data-ttu-id="f8b2f-139">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="f8b2f-139">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="f8b2f-140">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="f8b2f-140">certificateUploadStatus</span></span>|<span data-ttu-id="f8b2f-141">String</span><span class="sxs-lookup"><span data-stu-id="f8b2f-141">String</span></span>|<span data-ttu-id="f8b2f-142">証明書のアップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="f8b2f-142">The certificate upload status.</span></span>|
|<span data-ttu-id="f8b2f-143">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="f8b2f-143">certificateUploadFailureReason</span></span>|<span data-ttu-id="f8b2f-144">String</span><span class="sxs-lookup"><span data-stu-id="f8b2f-144">String</span></span>|<span data-ttu-id="f8b2f-145">理由の証明書のアップロードに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="f8b2f-145">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="f8b2f-146">証明書</span><span class="sxs-lookup"><span data-stu-id="f8b2f-146">certificate</span></span>|<span data-ttu-id="f8b2f-147">String</span><span class="sxs-lookup"><span data-stu-id="f8b2f-147">String</span></span>|<span data-ttu-id="f8b2f-148">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f8b2f-148">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8b2f-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f8b2f-149">Relationships</span></span>
<span data-ttu-id="f8b2f-150">なし</span><span class="sxs-lookup"><span data-stu-id="f8b2f-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f8b2f-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f8b2f-151">JSON Representation</span></span>
<span data-ttu-id="f8b2f-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f8b2f-152">Here is a JSON representation of the resource.</span></span>
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





