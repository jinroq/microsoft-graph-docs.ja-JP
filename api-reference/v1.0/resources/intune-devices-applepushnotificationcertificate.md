---
title: applePushNotificationCertificate リソースの種類
description: Apple プッシュ通知証明書。
ms.openlocfilehash: 7980f615d657b1c79dd09d1f5c06ced58151dbec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021445"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="d2eab-103">applePushNotificationCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d2eab-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="d2eab-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d2eab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2eab-105">Apple プッシュ通知証明書。</span><span class="sxs-lookup"><span data-stu-id="d2eab-105">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="d2eab-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d2eab-106">Methods</span></span>
|<span data-ttu-id="d2eab-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d2eab-107">Method</span></span>|<span data-ttu-id="d2eab-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d2eab-108">Return Type</span></span>|<span data-ttu-id="d2eab-109">説明</span><span class="sxs-lookup"><span data-stu-id="d2eab-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2eab-110">Get applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d2eab-110">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="d2eab-111">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d2eab-111">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="d2eab-112">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d2eab-112">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="d2eab-113">Update applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d2eab-113">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="d2eab-114">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d2eab-114">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="d2eab-115">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d2eab-115">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="d2eab-116">downloadApplePushNotificationCertificateSigningRequest 関数</span><span class="sxs-lookup"><span data-stu-id="d2eab-116">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="d2eab-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d2eab-117">String</span></span>|<span data-ttu-id="d2eab-118">Apple プッシュ通知の証明書署名要求をダウンロードします</span><span class="sxs-lookup"><span data-stu-id="d2eab-118">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="d2eab-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2eab-119">Properties</span></span>
|<span data-ttu-id="d2eab-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2eab-120">Property</span></span>|<span data-ttu-id="d2eab-121">型</span><span class="sxs-lookup"><span data-stu-id="d2eab-121">Type</span></span>|<span data-ttu-id="d2eab-122">説明</span><span class="sxs-lookup"><span data-stu-id="d2eab-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2eab-123">id</span><span class="sxs-lookup"><span data-stu-id="d2eab-123">id</span></span>|<span data-ttu-id="d2eab-124">String</span><span class="sxs-lookup"><span data-stu-id="d2eab-124">String</span></span>|<span data-ttu-id="d2eab-125">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="d2eab-125">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="d2eab-126">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="d2eab-126">appleIdentifier</span></span>|<span data-ttu-id="d2eab-127">String</span><span class="sxs-lookup"><span data-stu-id="d2eab-127">String</span></span>|<span data-ttu-id="d2eab-128">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="d2eab-128">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="d2eab-129">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="d2eab-129">topicIdentifier</span></span>|<span data-ttu-id="d2eab-130">String</span><span class="sxs-lookup"><span data-stu-id="d2eab-130">String</span></span>|<span data-ttu-id="d2eab-131">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="d2eab-131">Topic Id.</span></span>|
|<span data-ttu-id="d2eab-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2eab-132">lastModifiedDateTime</span></span>|<span data-ttu-id="d2eab-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2eab-133">DateTimeOffset</span></span>|<span data-ttu-id="d2eab-134">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="d2eab-134">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="d2eab-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d2eab-135">expirationDateTime</span></span>|<span data-ttu-id="d2eab-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2eab-136">DateTimeOffset</span></span>|<span data-ttu-id="d2eab-137">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="d2eab-137">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="d2eab-138">証明書</span><span class="sxs-lookup"><span data-stu-id="d2eab-138">certificate</span></span>|<span data-ttu-id="d2eab-139">String</span><span class="sxs-lookup"><span data-stu-id="d2eab-139">String</span></span>|<span data-ttu-id="d2eab-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d2eab-140">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2eab-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d2eab-141">Relationships</span></span>
<span data-ttu-id="d2eab-142">なし</span><span class="sxs-lookup"><span data-stu-id="d2eab-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2eab-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d2eab-143">JSON Representation</span></span>
<span data-ttu-id="d2eab-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d2eab-144">Here is a JSON representation of the resource.</span></span>
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



